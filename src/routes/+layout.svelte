<script lang="ts">
  import favicon from "$lib/assets/favicon.svg";
  import "@fontsource-variable/geist/wght.css";

  let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}

<style lang="scss">
	:global(body) {
		--background: #1f1f1f;
		--background-alt: #2c2c2c;
		--color: #fff;

		background: var(--background);
		color: var(--color);
		margin: 0px;
		padding: 0px;
	}

	:global(*) {
		font-family: 'Geist Variable', sans-serif;
	}
</style>
