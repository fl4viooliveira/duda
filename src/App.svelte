<script>
	import {onMount} from 'svelte';
	import {createScene} from "./scene.js";

	let webgl;

	onMount(() => {
		createScene(webgl)
	});
</script>

<canvas bind:this={webgl}></canvas>

<style>
	:global(body){
		margin: 0;
		padding: 0;
	}
</style>