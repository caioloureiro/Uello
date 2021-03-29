<template>

	<div class="Central_ajuda">

		<div class="Central_ajuda_txt">Central de Ajuda</div>
		
		<div class="Central_ajuda_icone">
		
			<svg
				version="1.1"
				id="Capa_1"
				xmlns="http://www.w3.org/2000/svg"
				xmlns:xlink="http://www.w3.org/1999/xlink"
				x="0px"
				y="0px"
				viewBox="0 0 256 256"
				style="enable-background:new 0 0 256 256;"
				xml:space="preserve"
			>
				<g>
					<g>
						<polygon points="225.813,48.907 128,146.72 30.187,48.907 0,79.093 128,207.093 256,79.093 		"/>
					</g>
				</g>
				<g></g><g></g><g></g><g></g><g></g><g></g><g></g><g></g><g></g><g></g><g></g><g></g><g></g><g></g><g></g>
			</svg>
			
		</div>
		
	</div>

</template>

<script>
export default {

	name: 'Central_ajuda',

}
</script>

<style scoped>

	.Central_ajuda{
		width:17.7vw;
		height:2.6vw;
		line-height:2.6vw;
		background-color:rgba(75, 75, 85,1);
		float:left;
		color:white;
		border-radius:0.3vw;
		margin-left:1vw;
		margin-top:1.4vw;
		cursor:pointer;
		font-size:0.9vw;
	}
	
	.Central_ajuda_icone{
		width:2.5vw;
		float:right;
		margin-left:1.5vw;
	}
	
	.Central_ajuda_txt{
		width:9vw;
		float:left;
		text-align:left;
		padding-left:4vw;
	}
	
	.Central_ajuda_txt:before{
		content:'';
		position:relative;
		width:1vw;
		height:2.5vw;
		background-image:url("../assets/img/information-white.svg");
		background-repeat:no-repeat;
		background-position:center center;
		background-size:100% auto;
		float:left;
		margin-right:0.5vw;
	}
	
	.Central_ajuda_icone svg{
		fill:white;
		width:1vw;
		height:auto;
		margin-top:0.8vw;
	}
	
	@media only screen and (max-width:1279px){
	
		.Central_ajuda{
			width:auto;
			height:9vw;
			line-height:9vw;
			background-color:rgba(75, 75, 85,1);
			float:right;
			color:white;
			border-radius:0.9vw;
			margin-right:5vw;
			margin-top:70vw;
			cursor:pointer;
			font-size:3vw;
			padding-left:3vw;
			padding-right:3vw;
		}
		
		.Central_ajuda_txt:before,
		.Central_ajuda_icone,
		.Central_ajuda_icone svg{
			display:none;
		}
		
		.Central_ajuda_txt{
			width:auto;
			text-align:center;
			padding-left:0vw;
		}
	
	}


</style>