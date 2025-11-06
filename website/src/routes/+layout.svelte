<script lang="ts">
	// import Header from './Header.svelte';

	import '../app.css';

	let { children } = $props();
</script>

<div class="app">
	<!--	<Header />-->

	<div class="window">Hello</div>

	<main>
		{@render children()}
	</main>
</div>

<style>
	.window {
		position: fixed;
		left: 50%;
		top: 50%;

		background-color: #1e2030;

		padding: 14px;

		width: 800px;
		height: 600px;

		border: 1px solid #181926;
		box-shadow: 0 0 20px #181926;

		border-radius: 8px;

		transform: translateX(-50%) translateY(-50%);
	}
</style>
