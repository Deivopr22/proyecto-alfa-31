<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<nav>
	<div>
		<span></span>
		<p>Studio</p>
	</div>

	<div>
		<a href="/">Home</a>
		<a href="/projects">Projects</a>
		<a href="/information">Information</a>
		<a href="/summary">Summary</a>
		<a href="/contact">Contact</a>
	</div>
</nav>


{@render children()}


<footer>
	Este es mi pie de página
</footer>