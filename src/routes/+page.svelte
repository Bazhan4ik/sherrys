<script lang="ts">
	import Header from "./c/header.svelte";
	import DressSection from "./c/dress-section.svelte";
</script>



<div class="app">
	<Header></Header>
	<DressSection></DressSection>
</div>

<style lang="scss">
	@use "../pallette.scss" as pallette;

	.app {
		width: 100%;
		background-color: pallette.$bg
	}

</style>
