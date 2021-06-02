<script>
	import { page } from '$app/stores';
	import Tabs from "smelte/src/components/Tabs";
	import AppBar from "smelte/src/components/AppBar";
	import Button from "smelte/src/components/Button";
	import { Spacer } from "smelte/src/components/Util"
	import IconButton from "../IconButton/index.svelte";

	$: path = $page ? $page.path ? $page.path : '/' : '/';
</script>

<AppBar classes="fixed top-0 w-screen items-center flex-wrap flex left-0 z-30 p-0 elevation-0 bg-dark-500 opacity-98" >
		<div class="w-4" style="height:52px"/>

		<IconButton icon="menu" />
		
		<Spacer/>

		<a href="/" class="flex items-center">
			<IconButton icon="video_call" />
		</a>
		<div style="width: 6px;"/>
		<a href="/about" class="flex items-center">
			<IconButton icon="account_circle" />
		</a>
		
		<div class="w-4" style="height:52px"/>
</AppBar>
<div style="height: 52px;" />