<script lang="ts">
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';
	
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>Fametonic: The Smart Way to Go Viral on Social Media</title>
</svelte:head>

{@render children?.()}
