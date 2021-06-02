<script>
	import { page } from '$app/stores';
	import Tabs from "smelte/src/components/Tabs";

	const topMenu = [
      { to: '/', text: 'Home' },
      { to: '/about', text: 'About' },
    ];

	$: path = $page.path ? $page.path : '/';
</script>

<header>
	<Tabs 
		items={topMenu} bind:selected={path} 
		class="bg-black shadow-sm mt-6 text-white"
		color="yellow-a200" />
</header>
