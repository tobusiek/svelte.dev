<script>
	const themes = ['margaritaville', 'retrowave', 'spaaaaace', 'halloween'];
	let selected = $state(themes[0]);
</script>

<svelte:head>
	<link rel="stylesheet" href="/tutorial/stylesheets/{selected}.css" />
</svelte:head>

<h1>Welcome to my site!</h1>

<select bind:value={selected}>
	<option disabled>choose a theme</option>

	{#each themes as theme}
		<option>{theme}</option>
	{/each}
</select>
