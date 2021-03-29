<template>

	<div class="Endereco_entrega">

		<div class="Endereco_entrega-icone"></div>
		<div class="Endereco_entrega-txt">
		
			Avenida Doutor Gastão Vidigal, 1132<br/>
			Vila Leopoldina - São Paulo - SP<br/>
			Apto - 1234 
		
		</div>
		
	</div>

</template>

<script>
export default {

	name: 'Endereco_entrega',

}
</script>

<style scoped>

	.Endereco_entrega{
		width:17.7vw;
		height:auto;
		background-color:rgba(255, 0, 0,0);
		float:left;
		margin-left:1vw;
		color:rgb(151,151,161);
		font-size:0.9vw;
		padding-bottom:0.5vw;
		text-align:left;
		margin-top:1vw;
		overflow:hidden;
	}
	
	.Endereco_entrega-icone{
		width:2vw;
		height:2vw;
		background-color:rgba(255,0,0,0);
		float:left;
		background-image:url("../assets/img/maps-and-flags.svg");
		background-repeat:no-repeat;
		background-position:center top;
		background-size:auto 1.5vw;
	}

	.Endereco_entrega-txt{
		width:15vw;
		height:auto;
		background-color:rgba(255,0,0,0);
		float:left;
	}
	
	@media only screen and (max-width:1279px){
	
		.Endereco_entrega{
			width:84vw;
			height:auto;
			background-color:rgba(255, 255, 255,1);
			float:left;
			margin-left:5vw;
			border-radius:3vw;
			color:rgb(151,151,161);
			font-size:3vw;
			padding:3vw;
			text-align:left;
			margin-top:5vw;
			margin-bottom:15vw;
			overflow:hidden;
			box-shadow: 1vw 0.3vw 1.5vw rgba(0,0,0,0.2);
		}
		
		.Endereco_entrega-icone{
			width:12vw;
			height:12vw;
			background-color:rgba(255,0,0,0);
			float:left;
			background-image:url("../assets/img/maps-and-flags.svg");
			background-repeat:no-repeat;
			background-position:center top;
			background-size:auto 9vw;
		}

		.Endereco_entrega-txt{
			width:72vw;
			height:auto;
			background-color:rgba(255,0,0,0);
			float:left;
			line-height:6vw;
		}
	
	}


</style>