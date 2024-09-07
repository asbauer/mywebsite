<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
	import linkedin from '$lib/images/linkedin.png'
	import gmail from '$lib/images/gmail.png'
</script>

<header>
	<div hidden class="corner lg-view">
		<a hidden href="https://kit.svelte.dev">
			<img hidden src={logo} alt="SvelteKit" />
		</a>
	</div>

	<nav>
		<svg class="lg-view" viewBox="0 0 2 3" aria-hidden="true">
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
			<li id="contact" aria-current={$page.url.pathname.startsWith('/sverdle') ? 'page' : undefined}>
				<a href="/contact">Contact</a>
			</li>
			<li id="resume" aria-current={$page.url.pathname.startsWith('/sverdle') ? 'page' : undefined}>
				<a href="/resume">Resume</a>
			</li>


		</ul>
		<svg class="lg-view" viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z" />
		</svg>
	</nav>

	<div id="corner-socials">
		<a href="mailto:abauer121@gmail.com">
			<img src={gmail} alt="Gmail" />
		</a>
		<a href="https://www.linkedin.com/in/asbauer/">
			<img src={linkedin} alt="LinkedIn"/>
		</a>
		<a href="https://github.com/asbauer">
			<img src={github} alt="GitHub"  />
		</a>
	
		
	</div>
</header>

<style>


@media screen and (min-width:501px) {
	#contact {
		display: none;
	}
}
 


/*
	img {
		min-width: 100%;
		max-height: 100%;
	}
	*/


	header {
		display: flex;
		justify-content: space-between;
		
		
	}

	.corner,#corner-socials {
		display: flex;
		width: 3em;
		height: 3em;
		object-fit: contain;
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
		align-self: center;

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
	

	

	
	@media screen and (max-width:500px) {
		#corner-socials, img, .lg-view{
			display: none;
		}

		ul {
			width: 100%;
			justify-content: space-evenly;
		}

		nav {
			width: 100%;
		}

		nav a{
			padding: 0% 1% 0% 1%;
			
			
		}
/*
		li {
			margin-left: 2% ;
			margin-right: 2%;
		}

		ul li:first-child {
			padding-left: 2.5%;
			margin-right: 2%;

		}

		ul li:last-child {
			padding-right: 2.5%;
			margin-left: 2%;
			
		}
			*/

		nav {
			justify-content: space-evenly;
		}

		a {
			font-size: x-small;
		}
		

	
		
	}

	@media screen and (max-width:330px) {
		nav a {
			font-size: x-small
		}
	}



	
</style>
