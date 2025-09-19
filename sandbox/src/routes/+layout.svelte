<script>
	import favicon from '$lib/assets/favicon.svg';
	import Component from '$lib/components/Component.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>


<nav>
	<a href="/">index</a>
	<a href="/details">details</a>
	<a href="/team">team</a>
	<a href="/about">about</a>
</nav>





<Component/>


{@render children?.()}


<footer style="color: purple;">
	<h2> dit is de footer</h2>
</footer>


<style>
	a {
		color: darkgreen;
	}
</style>