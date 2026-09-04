<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import Icon from '@iconify/svelte';

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
	<div>© 2024 Studio. All rights reserved.</div>

	<div>
		<a href="https://www.linkedin.com/in/deivis-p%C3%A9rez-444045342/">LinkedIn</a>
		<a href="https://github.com/Deivopr22">GitHub</a>
		<a href="https://www.instagram.com/deivopr22/">Instagram</a>

	</div>
</footer>