<script>
	export let src;
	export let title = '';
</script>

<div class="wrap">
	<div style={`background-image:url("${src}")`} class="derp" />
	<p class="title">{title}</p>
</div>

<style>
	.wrap {
		margin: 20px;
	}
	.title {
		text-align: center;
		color: #555;
	}
	.derp {
		width: 250px;
		height: 400px;
		border: 4px solid purple;
		border-radius: 8px;

		background-position: center;
		background-size: cover;
	}
</style>
