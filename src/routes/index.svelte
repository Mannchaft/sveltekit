<script>
	import { pokemon } from '../stores/equipment-store';
	console.log($pokemon);
</script>

<svelte:head>
	<title>Admin-Kit</title>
</svelte:head>
<body>
	<div class="center">
		<h1>Welcome to Admin-Kit</h1>
	</div>
	{#each $pokemon as pokeman}
		<p>{pokeman.name}</p>
	{/each}
</body>

<style lang="scss">
	@import '../styles/vars';
	@import '../styles/css';
</style>
