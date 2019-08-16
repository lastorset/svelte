<script>
	import Thing from './Thing.svelte';

	let things = [
		{ id: 1, value: 'skyblue' },
		{ id: 2, value: 'thistle' },
		{ id: 3, value: 'pink' },
		{ id: 4, value: 'linen' },
		{ id: 5, value: 'gold' }
	];

	function handleClick() {
		things = things.slice(1);
	}
</script>

<button on:click={handleClick}>
	Remove first thing
</button>

{#each things as thing}
	<Thing value={thing.value}/>
{/each}