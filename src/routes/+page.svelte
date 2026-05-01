<script lang="ts">
	import Item1 from "./items/item1.svelte";
</script>



<div class="app">
	<div class="header">
		<h1>Sherry's</h1>
	</div>
	<Item1></Item1>

</div>

<style lang="scss">

	.app {
		width: 100%;
	}
	.header {
		height: 160px;
		width: 100%;
		display: flex;
		justify-content: center;
		align-items: center;

		h1 {
			font-family: "Tangerine", cursive;
			font-size: 3rem;
		}
	}


</style>
