<script>
	import Header from '../components/Header.svelte';
	import Imagine from '../components/Imagine.svelte';

	let images = [
		{ src: '/canal-walk.jpg' },
		{ src: '/colorful-markers.jpg' },
		{ src: '/guitars.jpg' },
		{ src: '/paints.jpg' },
		{ src: '/tye-dye.jpg' },
		{ src: '/zebra-with-robbie.jpg' }
	];
</script>

<Header />

<div class="format">
	{#each images as image}
		<Imagine src={image.src} />
	{/each}
</div>

<style>
	.format {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
		margin: 0 2rem;
	}
</style>
