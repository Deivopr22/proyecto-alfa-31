<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import Icon from '@iconify/svelte';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<nav class = "flex justify-between items-baseline p-4 bg-gray-100 shadow-md">
	<div class="flex">
		<a href="/" class="font-montserrat text-md tracking-widest font-bold uppercase">studio</a>
	</div>

	<div class ="flex gap-5 text-gray-600 text-xs justify-center items-center tracking-widest uppercase">
		<a href="/" class="font-montserrat font-bold underline underline-offset-1 hover:text-black">Home</a>
		<a href="/projects" class="font-montserrat font-bold underline underline-offset-1 hover:text-black">Projects</a>
		<a href="/information" class="font-montserrat font-bold underline underline-offset-1 hover:text-black">Information</a>
		<a href="/summary" class="font-montserrat font-bold underline underline-offset-1 hover:text-black">Summary</a>
		<a href="/contact" class="font-montserrat font-bold underline underline-offset-1 hover:text-black">Contact</a>
	</div>
</nav>

<hr class="border-gray-300 border-t-2 w-full"/>

{@render children()}

<hr class="border-gray-300 border-t-2 w-full shadow-lg"/>
<footer class = "flex justify-between items-center p-4 bg-gray-200 text-xs">

	<div class="font-montserrat font-bold">© 2024 Studio. All rights reserved.</div>

	<div class="flex gap-6 text-gray-600">
		<a href="https://www.linkedin.com/in/deivis-p%C3%A9rez-444045342/" class="underline	underline-offset-3 hover:text-black">LinkedIn</a>
		<a href="https://github.com/Deivopr22" class="underline	underline-offset-3 hover:text-black">GitHub</a>
		<a href="https://www.instagram.com/deivopr22/" class="underline	underline-offset-3 hover:text-black">Instagram</a>

	</div>
</footer>

