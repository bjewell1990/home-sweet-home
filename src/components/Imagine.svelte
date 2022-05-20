<script>
	export let src;
</script>

<div style={`background-image:url("${src}")`} class="derp" />

<style>
	.derp {
		width: 250px;
		height: 400px;
		border: 4px solid purple;
		border-radius: 8px;
		margin: 20px;
		background-position: center;
		background-size: cover;
	}
</style>
