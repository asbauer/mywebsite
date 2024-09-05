<script>/*
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
    */
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

	<h1>
		Welcome
	</h1>


	<div class="loader">
        <div class="dot"></div>
        <div class="dot"></div>
        <div class="dot"></div>
    </div>



<style>
	 .loader {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .loader .dot {
            width: 16px;
            height: 16px;
            margin: 0 8px;
            border-radius: 50%;
            background: #333;
            animation: bounce 1.2s infinite ease-in-out;
        }

        .loader .dot:nth-child(2) {
            animation-delay: 0.2s;
        }

        .loader .dot:nth-child(3) {
            animation-delay: 0.4s;
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0);
            }
            40% {
                transform: translateY(-24px);
            }
            60% {
                transform: translateY(-12px);
            }
        }





	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
