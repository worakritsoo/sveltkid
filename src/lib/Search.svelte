<script>
	import Fuse from 'fuse.js';
	import links from './links.json';
	export let value = 'wor';
	const map = new Map([
		['name', 'Svelte'],
		['link', 'JavaScript']
	]);

	const fuse = new Fuse(links, {
		keys: ['name', 'title'],
		includeScore: true
	});
	$: res = fuse.search(value);
	const results = fuse.search(`${value}`);
	let linkResults = [...results];
	console.log(results);
</script>

<input type="search" bind:value placeholder="Search . . ." />

<!-- markup (zero or more items) goes here -->
{JSON.stringify(res)}

<style>
	/* your styles go here */
</style>
