<script lang="ts">
	import IMG_full from "$lib/assets/picture1_full.jpg";
</script>


<div class="app">

	<div class="large-image">
		<div class="header">
			<div class="big">
				<p>Dress Season is Here</p>
			</div>
			<div class="small">
				<a href="">SHOP NOW</a>
			</div>
			<div class="center">
				<span class="material-symbols-rounded"> arrow_drop_down </span>
				<div class="small">
					<p>See our new dresses</p>
				</div>
				<span class="material-symbols-rounded"> arrow_drop_down </span>
			</div>
		</div>
		<div class="image-container">
			<img src={IMG_full} alt="pic1">
		</div>
	</div>
</div>


<style lang="scss">
	.app {
		width: 100%;
		overflow: visible;
	}

	.large-image {
		width: 100%;
		position: relative;
		overflow: visible;
	}

	$header-height: 142px;
	$header-to-bottom: 12px;
	.header {
		$header-padding-left: 24px;

		position: absolute;
		bottom: $header-to-bottom;
		left: 0;
		z-index: 1;
		width: 100%;
		min-height: $header-height;
		overflow: visible;
		display: flex;
		flex-direction: column;
		gap: 12px;

		.big p {
			font-family: "Quintessential", serif;
			font-size: 1.4rem;
			color: white;
			letter-spacing: 3px;
			padding-left: $header-padding-left;
		}
		.small a, .small p {

			padding-left: $header-padding-left;
			font-family: "Quintessential", serif;
			font-size: 1.0rem;
			color: rgb(200, 200, 200);
			letter-spacing: 3px;
		}
		.small a {
			text-decoration: underline;
		}
		.center {
			display: flex;
			justify-content: center;
			gap: 8px;
			margin-top: 24px;
			.small p { font-size: 0.95rem; padding-left: 0; color: rgb(180, 180, 180); }
			span {
				display: flex; justify-content: center; align-items: center;
				color: rgb(180, 180, 180);
				font-size: 1.6rem;
			}
		}
	}
	.image-container {
		width: 100%;
		position: relative;
		display: inline-block;
		z-index: 0;

		&::after {
			content: "";
			position: absolute;
			top: 0; left: 0;
			width: 100%; height: calc(100%);
			background: linear-gradient(to bottom, rgba(black, 0.3) 0%, transparent 15%, transparent 60%, rgba(black, 0.6) calc(100% - $header-to-bottom - $header-height), rgba(black, 0.6) 100%);
			// background: linear-gradient(to bottom, rgba(#caa798, 0.8) 0%, transparent 15%);
		}
	}
	.image-container img {
		display: block;
		width: 100%;
		z-index: 0;
	}
</style>


