<script lang="ts">
	import '@picocss/pico';
</script>

<svelte:head>
  <link href="https://fonts.googleapis.com/css?family=Roboto:400,700" rel="stylesheet">
</svelte:head>
<main class="container">
	<article>
		<header>Header</header>
		<slot />
		<footer>Footer</footer>
	</article>
</main>

<style>
	:global(body) {
		font-family: 'Roboto', sans-serif;
	}
	article {
		text-align: justify;
	}
</style>
