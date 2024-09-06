<script>
	import Header from './Header.svelte';
	import './styles.css';
	
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
    <hr>
    <p>&copy;2024 Adam Bauer. All Rights Reserved. 
	</p>
	<a id="email-attribution" href="https://www.flaticon.com/free-icons/gmail" title="gmail icons">Gmail icons created by Pixel perfect - Flaticon</a>
</footer>
</div>

<style>

	a#email-attribution{
		color: var(--color-text,rgb(244, 229, 212));
		text-decoration: none;
		font-weight: 400;
	}

	footer {
    text-align: center;
	}

	footer p {
		margin-top: 0.3%;
	}

	hr {
    border: 1px solid brown;
	width: 100%;
	}
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}



	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}

	@media  screen and (max-width:500px){
		main {
			padding-left: 0;
			padding-right: 0;
		}

	 }
</style>
