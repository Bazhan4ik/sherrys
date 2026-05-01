<script lang="ts">
	import IMG1 from "$lib/assets/item1.png"

</script>


<section id="dress-items" class="app">
	<button class="product">
		<div class="image-container">
			<img src={IMG1} alt="">
		</div>
		<div class="info">
			<div class="product-name">Coral Dress</div>
			<div class="product-price">$110.99</div>
		</div>
	</button>
	<button class="product">
		<div class="image-container">
			<img src={IMG1} alt="">
		</div>
		<div class="info">
			<div class="product-name">Coral Dress</div>
			<div class="product-price">$110.99</div>
		</div>
	</button>
	<button class="product">
		<div class="image-container">
			<img src={IMG1} alt="">
		</div>
		<div class="info">
			<div class="product-name">Coral Dress</div>
			<div class="product-price">$110.99</div>
		</div>
	</button>
	<button class="product">
		<div class="image-container">
			<img src={IMG1} alt="">
		</div>
		<div class="info">
			<div class="product-name">Coral Dress</div>
			<div class="product-price">$110.99</div>
		</div>
	</button>

</section>

<style lang="scss">
	@use "./../../pallette.scss" as pallette;
	.app {
		padding: 24px 20px 36px;
		display: grid; gap: 24px; grid-template-columns: 1fr 1fr;
	}

	button.product {
		aspect-ratio: 3 / 4;
		background: none; border: none;
		cursor: pointer;
		display: flex; flex-direction: column; align-items: flex-start;
	}

	.image-container {
		background-color: pallette.$paper;
	}
	.image-container, img {
		border-radius: 8px;
		width: 100%;
		height: 100%;
		object-fit: cover;
	}

	.info {
		margin-top: 10px;
		display: flex; flex-direction: column; align-items: flex-start;
	}

	.info .product-name {
		font-family: "Cormorant Garamond", serif; font-size: 1rem; font-style: italic;
		line-height: 1.2;
	}
	.info .product-price {
		font-family: "Inter", serif; font-size: 0.625rem; font-variant-numeric: "tabular-nums";
		color: pallette.$muted;
	}


</style>
