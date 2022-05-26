<script>
	import Header from '../components/Header.svelte';
	import Imagine from '../components/Imagine.svelte';

	let images = [
		{ src: '/canal-walk.jpg', title: 'A beautiful day on the canal' },
		{ src: '/colorful-markers.jpg', title: 'Colorful Markers' },
		{ src: '/guitars.jpg', title: 'Colorful Guitars' },
		{ src: '/paints.jpg', title: 'Painting day' },
		{ src: '/tye-dye.jpg', title: 'Tye-Dye high dye' },
		{ src: '/zebra-with-robbie.jpg', title: 'Zebra with Robbie' },
		{ src: '/Buttons.jpeg', title: 'Colorful Buttons' },
		{ src: '/Fruit.jpeg', title: 'Colorful Fruit' },
		{ src: '/Colorful-wow.jpeg', title: 'Colorful wow' },
		{ src: '/Ice-Cream.jpeg', title: 'Ice Cream Shop' },
		{ src: '/Im on the boat.jpeg', title: "I'm on a boat!" },
		{ src: '/Umbrellas.jpeg', title: 'Colorful Umbrellas' }
	];
</script>

<Header />

<div class="format">
	{#each images as image}
		<Imagine src={image.src} title={image.title} />
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
