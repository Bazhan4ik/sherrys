<script lang="ts">
	import IMG from "$lib/assets/picture1.jpg";
	import IMG_full from "$lib/assets/picture1_full.jpg";
	import IMG_item1 from "$lib/assets/item1.png";
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


	<!-- <div class="items"> -->
	<!-- 	<div class="header"> -->
	<!-- 		<p>Easy, flattering fits</p> -->
	<!-- 	</div> -->
	<!-- 	<div class="item"> -->
	<!-- 		<div class="image"> -->
	<!-- 			<img src={IMG_item1} alt="item1"> -->
	<!-- 		</div> -->
	<!-- 		<div class="info"> -->
	<!-- 			<div class="name"><p>Flowy florals</p></div> -->
	<!-- 		</div> -->
	<!-- 	</div> -->
	<!-- </div> -->


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
		position: absolute;
		bottom: $header-to-bottom;
		left: 0;
		z-index: 1;
		width: 100%;
		min-height: $header-height;
		overflow: visible;
		display: flex;
		flex-direction: column;
		padding-left: 24px;
		gap: 12px;

		.big p {
			font-family: "Quintessential", serif;
			font-size: 1.4rem;
			color: white;
			letter-spacing: 3px;
		}
		.small a, .small p {
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
			.small p { font-size: 0.95rem; color: rgb(180, 180, 180); }
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

	.items {
		position: relative;
		z-index: 1;
		padding-top: 120px;
		width: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
		width: 100%;
		background-color: #79645b;

		background: linear-gradient(0deg,rgba(#79645b, 1) calc(100% - 80px), rgba(255, 255, 255, 0) 100%);
		margin-top: -100px;
	}

	.items .header {
		background-color: #79645b;
		box-shadow: none;
		p {
			color: #e5d3cc;
			font-family: "Quintessential", serif;
			letter-spacing: 0;
		}
	}
	.item {
		// margin-top: -80px;
		max-width: 300px;
		width: 100%;
		background-color: #efe5e0;

		.image {
			display: flex;
			justify-content: center;
			align-items: center;
			width: 100%;
		}
		.image img {
			width: 100%;
			max-width: 200px;
		}
	}
	
</style>


