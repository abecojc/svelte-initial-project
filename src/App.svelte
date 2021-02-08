<script>
    import Nested from './Nested.svelte';
    export let name;
    let src = "tutorial/image.gif";
	name = 'Rick Astley';
</script>

<main>
	<h1>Hello {name.toUpperCase()}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
    <img src = { src } alt=" { name } dances.">
    <p> This is a paragraph.</p>
    <Nested/>
</main>

<style>
    p{
        color: purple;
        font-family: 'Comic Sans MS', cursive;
        font-size: 2em;
    }
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