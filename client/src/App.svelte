<script>
	import { Router, Link, Route, navigate} from 'svelte-routing'
	import { onMount } from "svelte";
	import Dashboard from './pages/Dashboard.svelte';
	import LogIn from './pages/LogIn.svelte';
	import Admin from './pages/Admin.svelte';
	import Archive from './pages/Archive.svelte';
	export let url = '';

</script>

<main>
	<Router url="{url}">
	<div>
		<Route path="/" component="{LogIn}" />
		<Route path="/dashboard" component="{Dashboard}" />
		<Route path="/admin" component="{Admin}" />
		<Route path="/archive" component="{Archive}" />
	</div>
	</Router>
</main>

