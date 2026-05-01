<script lang="ts">
	import Header from "./c/header.svelte";
	import DressSection from "./c/dress-section.svelte";
	import DressItemsSection from "./c/dress-shop.svelte";
</script>



<div class="app">
	<Header></Header>
	<DressSection></DressSection>
	<DressItemsSection></DressItemsSection>
</div>

<style lang="scss">
	@use "../pallette.scss" as pallette;

	.app {
		width: 100%;
		background-color: pallette.$bg
	}

</style>
