<script context="module">
	export const prerender = true;
</script>

<script>
	import Counter from '$lib/Counter.svelte';
	import JordanPeterson from './/JordanPeterson.svelte';
	import MusicAndVisions from './MusicAndVisions.svelte';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section>
	<h1>
		Life Sanctuary
	</h1>

	<JordanPeterson/>
	<MusicAndVisions/>

	TODO: 
		2. Memory drawings and history
	  3. Fun places and things to do

	<!-- <Counter /> -->
	
	<!-- <div class="welcome">
		<picture>
			<source srcset="svelte-welcome.webp" type="image/webp" />
			<img src="svelte-welcome.png" alt="Welcome" />
		</picture>
	</div> -->
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
	}

	.welcome {
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
