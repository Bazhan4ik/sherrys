<script lang="ts">
	import Item1 from "./items/item1.svelte";
</script>



<div class="app">
	<div class="header">
		<div class="title">
			<h1>Sherry's</h1>
		</div>
		<div class="links">
			<div class="link">
				<a href="">Dresses</a>
			</div>
			<div class="link">
				<a href="">Hats</a>
			</div>
			<div class="link">
				<a href="">Jewelry</a>
			</div>
		</div>
	</div>
	<Item1></Item1>
</div>

<style lang="scss">

	.app {
		width: 100%;
	}
	.header {
		width: 100%;
		display: flex;
		align-items: center;
		flex-direction: column;
		box-shadow: 0px -5px 5px -5px rgba(34, 60, 80, 0.6) inset;
		overflow: visible;
		z-index: 2;

		.title {
			display: flex;
			align-items: center;
			justify-content: center;
			padding-top: 24px;
			padding-bottom: 12px;
			border-bottom: 1px solid rgb(230, 230, 230);
			width: 100%;

		}
		.title h1 {
			font-family: "Tangerine", cursive;
			font-size: 3rem;
		}
	}

	.header .links {
		display: flex;
		justify-content: space-between;
		width: 100%;

		.link {
			width: 100%;
			height: 42px;
			display: flex;
			align-items: center;
			justify-content: center;

			a {
				font-family: "Quintessential", serif;
				font-size: 1.0rem;
				text-decoration: none;
				color: black;
			}
		}
	}


</style>
