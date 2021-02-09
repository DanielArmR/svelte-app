<script>
	export let name;
	let userName = 'Daniel';
	import Counter from './Counter.svelte';
	import Form from './Form.svelte';
</script>

<main>
	<h1>Hello {name}!</h1>
	<h2>Welcome {userName} to Svelte</h2>
	<Counter counter={2}/>
	<Counter counter={10}/>
	<Form />
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>