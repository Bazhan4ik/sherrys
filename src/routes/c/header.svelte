
<header>
	<button class="mobile-menu-btn" aria-label="mobile-menu">
		<svg width="20" height="14" viewBox="0 0 20 14" fill="none" stroke="currentColor">
			<path d="M0 1h20M0 7h20M0 13h20" />
		</svg>
	</button>
	<button class="home-btn">Sherry's</button>
</header>

<style lang="scss">
	@use "./../../pallette.scss" as pallette;

	.app {
		width: 100%;
	}

	header {
		width: 100%;
		display: flex; align-items: center; justify-content: flex-start; gap: 20px;
		flex-shrink: 0;
		padding: 14px 20px;
		border-bottom: 1px solid pallette.$line;
		background: pallette.$bg;
	}

	.mobile-menu-btn {
		background: none; border: none;
		padding: 8px;
		color: pallette.$ink;
		cursor: pointer;
	}

	.home-btn {
		background: transparent; border: none;
		cursor: pointer;
		font-family: "Cormorant Garamond", serif; font-size: 1.625rem; font-weight: 400;
		color: pallette.$ink;
		font-style: italic;
	}



</style>
