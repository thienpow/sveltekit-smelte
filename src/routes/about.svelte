<script>
	import List from "smelte/src/components/List";
	
	const listOneLine = [{
		text: 'Item 1',
		icon: 'favorite',
	}, {
		text: 'Item 2',
		icon: 'favorite',
	}, {
		text: 'Item 3',
		icon: 'favorite',
	}];
	
	const listTwoLines = [{
		text: 'Item 1',
		icon: 'favorite',
		subheading: 'Subheading 1',
	}, {
		text: 'Item 2',
		icon: 'favorite',
		subheading: 'Subheading 2',
	}, {
		text: 'Item 3',
		icon: 'favorite',
		subheading: 'Subheading 3',
	}];

	let selected = false;
</script>

<svelte:head>
	<title>Sample List</title>
</svelte:head>
<h1>Sample List</h1>
<h6 class="mb-3 mt-6">One-line</h6>
<List items={listOneLine} />
<h6 class="mb-3 mt-6">Two-line</h6>
<List items={listTwoLines} />

<h6 class="mb-3 mt-6">Dense</h6>
<List dense items={listTwoLines} />

