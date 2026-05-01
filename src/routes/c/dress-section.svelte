<script lang="ts">
	import IMG from "$lib/assets/picture1_full.jpg"


</script>

<section id="dresses" class="app">
	<div class="date">April 25</div>
	<h1 class="dresses-title">Just in: <br> <em>spring dresses</em>, <br> fresh on the floor.</h1>
	<p class="dresses-subtitle">Hand-picked florals, breezy silhouettes, and easy everyday pieces. Try on at the shop.</p>

	<img src={IMG} alt="new-dresses">


</section>

<style lang="scss">
	@use "./../../pallette.scss" as pallette;

	.app {
		padding: 32px 20px 8px;
	}
	.date {
		font-size: 0.625rem; letter-spacing: 0.28rem; font-family: "Inter", sans-serif;
		text-transform: uppercase;
		color: pallette.$muted;
		margin-bottom: 16px;
	}
	h1.dresses-title {
		font-family: "Cormorant Garamond", serif; font-size: 3.5rem; font-weight: 400;
		line-height: 0.95; letter-spacing: -0.02rem;
	}
	p.dresses-subtitle {
		font-size: 0.875rem; font-family: "Inter", sans-serif;
		line-height: 1.7;
		color: pallette.$muted;
		margin-top: 18px;
		max-width: 380px;
	}

	img {
		width: 100%;

	}

</style>
