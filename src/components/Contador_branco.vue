<template>

	<div class="Contador_branco">
	
		<div class="Contador_branco-marcador"></div>
	
		<div class="Contador_branco-icone">
		
			<div class="Contador_branco-icone-txt">
				Falta<br/>
				<span>1</span><br/>
				Entrega
			</div>
		
		</div>
		
		<div class="Contador_branco-txt">
		
			Sua entrega é a n°: <span>19</span><br/>
			Entrega Atual: 18<br/>
			Quantidade de volumes: 3<br/>
			Motorista: Vinkius Marques do Nascimento<br/>
			Horário Estimado: 15:29 - 16:29 
		
		</div>
	
	</div>

</template>

<script>
export default {

	name: 'Contador_branco',

}
</script>

<style scoped>

	.Contador_branco{
		background-color:rgba(255, 0, 0,0);
		width:17.7vw;
		height:auto;
		float:left;
		margin-left:1vw;
		color:rgb(150,150,160);
		font-size:0.95vw;
		padding-bottom:0.5vw;
	}
	
	.Contador_branco-icone{
		width:6vw;
		height:8vw;
		background-color:rgba(255,255,255,1);
		float:left;
		background-image:url("../assets/img/loading-process.svg");
		background-repeat:no-repeat;
		background-position:center center;
		background-size:6vw auto;
	}
	.Contador_branco-icone-txt{
		width:3.8vw;
		height:3.8vw;
		background-color:rgba(255,255,255,0);
		float:left;
		margin-left:1.1vw;
		margin-top: 2.2vw;
		font-size: 0.7vw;
		border-radius: 5vw;
		line-height: 1.1vw;
	}
	.Contador_branco-icone-txt span{
		font-size: 1vw;
		line-height: 1.2vw;
		font-weight:bold;
	}
	.Contador_branco-txt span{
		color:red;
		font-weight:bold;
	}
	.Contador_branco-txt{
		width:10.7vw;
		height:8vw;
		background-color:rgba(255,255,255,1);
		float:left;
		text-align:left;
		color:rgb(150,150,160);
		padding-top:1vw;
		padding-left:1vw;
		font-size: 0.7vw;
	}
	
	.Contador_branco-marcador{
		position:absolute;
		width:5.7vw;
		height:0.2vw;
		background-color:rgba(11, 79, 108,1);
		margin-left:6vw;
	}
	
	@media only screen and (max-width:1279px){
	
		.Contador_branco{
		}
	
	}


</style>