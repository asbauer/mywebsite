<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
	import linkedin from '$lib/images/linkedin.png'
	import gmail from '$lib/images/gmail.png'
</script>

<header>
	<div hidden class="corner">
		<a hidden href="https://kit.svelte.dev">
			<img hidden src={logo} alt="SvelteKit" />
		</a>
	</div>

	<nav>
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z" />
		</svg>
		<ul>
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">Home</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">About</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/sverdle') ? 'page' : undefined}>
				<a href="/portfolio">Portfolio</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/sverdle') ? 'page' : undefined}>
				<a href="/contact">Contact</a>
			</li>

		</ul>
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z" />
		</svg>
	</nav>

	<div id="corner-socials">
		<a href="mailto:abauer121@gmail.com">
			<img src={gmail} alt="Gmail" />
		</a>
		<a href="https://www.linkedin.com/in/asbauer/">
			<img src={linkedin} alt="LinkedIn" />
		</a>
		<a href="https://github.com/asbauer">
			<img src={github} alt="GitHub" />
		</a>
	
		
	</div>
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		
	}

	.corner,#corner-socials {
		display: flex;
		width: 3em;
		height: 3em;
	}

	#corner-socials {
		display: flex;
		width:5em;
		height: 3em;
		justify-content: space-between;
	}

	
	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	#corner-socials a {
		display: flex;
		margin: 5%;
	}

	.corner img {
		width: 2em;
		height: 2em;
		object-fit: contain;
	
	}
		

	#corner-socials img {
		width: 100%;
		height: 100%;
		object-fit: contain;
		
	}
		

	nav {
		display: flex;
		justify-content: center;
		--background: rgba(255, 255, 255, 0.7);
		--background:rgba(18, 69, 126, 0.7);

		justify-self: center;
		text-align: center;

	}

	svg {
		width: 2em;
		height: 3em;
		display: block;
	}

	path {
		fill: var(--background);
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page']::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-1);
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
		transition: transform 0.3s ease;
		/*background-color:navy;
		*/
	}

	a:hover {
		color: var(--color-theme-1);
		color: brown;
		size: 2rem;
		transform:scale(1.1);
		
	

	}

	

	

	
</style>
