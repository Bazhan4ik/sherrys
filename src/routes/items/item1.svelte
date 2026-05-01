<script lang="ts">
	import IMG from "$lib/assets/picture1.jpg";
	import IMG_item1 from "$lib/assets/item1.png";
</script>


<div class="app">
	<div class="header">
		<p>
			DRESS SEASON IS HERE
		</p>
	</div>
	<div class="big-image">
		<img src={IMG} alt="pic1">
	</div>

	<div class="items">
		<div class="header">
			<p>Easy, flattering fits</p>
		</div>
		<div class="item">
			<div class="image">
				<img src={IMG_item1} alt="item1">
			</div>
			<div class="info">
				<div class="name"><p>Flowy florals</p></div>
			</div>
		</div>
	</div>


</div>


<style lang="scss">
	.app {
		width: 100%;
		overflow: visible;
	}
	.header {
		width: 100%;
		height: 64px;
		background-color: #caa798;
		overflow: visible;
		box-shadow: 0px -5px 18px 2px rgba(#caa798, 0.6);
		display: flex;
		justify-content: center;
		align-items: center;

		p {
			font-family: "Lobster", sans-serif;
			font-size: 1.2rem;
			color: #51433d;
			letter-spacing: 3px;
		}
	}
	.big-image {
		width: 100%;
		position: relative;
		z-index: 0;

		&::after {
			content: "";
			position: absolute;
			top: 0; left: 0;
			width: 100%; height: calc(100%);
			background: linear-gradient(to bottom, #caa798 0%, transparent 20%);
		}
	}
	.big-image img {
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


