<script lang="ts">
	import '../styles/app.css';
	import Header from '$components/Header.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<title>Sveltype</title>
</svelte:head>

<Header />

<div class="p-8 h-full">
	<main>
		{@render children()}
	</main>
</div>

<div>
	<a class="absolute right-10 bottom-12 text-lg" href="https://github.com/rcb123/sveltype"
		>&lt;/&gt; GitHub</a
	>
	<a class="absolute right-10 bottom-5 text-lg" href="https://rezab.vercel.app/">🖥️ Portfolio</a>
</div>

<style>
	/* lexend-deca-regular - latin */
	@font-face {
		font-family: 'Lexend Deca';
		font-style: normal;
		font-weight: 400;
		src:
			local(''),
			url('$static/fonts/lexend-deca-v17-latin/lexend-deca-v17-latin-regular.woff2') format('woff2'),
			url('$static/fonts/lexend-deca-v17-latin/lexend-deca-v17-latin-regular.woff') format('woff');
	}
</style>
