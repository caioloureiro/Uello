<template>

	<div class="Contador_azul">
		
		<div class="Contador_azul-marcador"></div>
	
		<div class="Contador_azul-icone">
		
			<div class="Contador_azul-icone-txt">
				Falta<br/>
				<span>1</span><br/>
				Entrega
			</div>
		
		</div>
		
		<div class="Contador_azul-trajeto">
			
			<div class="Trajeto-bloco-inicio bloco-01 concluido">
		
				<div class="Trajeto-icone"></div>
				<div class="Trajeto-marcador"></div>
				<div class="Trajeto-txt">Solicitação</div>
			
			</div>
			<div class="Trajeto-bloco bloco-02 concluido">
			
				<div class="Trajeto-linha"></div>
				<div class="Trajeto-icone"></div>
				<div class="Trajeto-marcador"></div>
				<div class="Trajeto-txt">Pedido em separação</div>
			
			</div>
			<div class="Trajeto-bloco bloco-03 concluido">
			
				<div class="Trajeto-linha"></div>
				<div class="Trajeto-icone"></div>
				<div class="Trajeto-marcador"></div>
				<div class="Trajeto-txt">Motorista em trânsito</div>
			
			</div>
			<div class="Trajeto-bloco bloco-04">
			
				<div class="Trajeto-linha"></div>
				<div class="Trajeto-icone"></div>
				<div class="Trajeto-marcador"></div>
				<div class="Trajeto-txt">Pedido entregue</div>
			
			</div>
		
		</div>
		
		<div class="Contador_azul-txt">
		
			Status do pedido: Saiu para entrega<br/>
			Horário estimado: 15:29 - 16:29
		
		</div>
		
	</div>

</template>

<script>
export default {

	name: 'Contador_azul',

}
</script>

<style scoped>

	@media only screen and (max-width:1279px){
	
		.Contador_azul{
			width:90vw;
			height:auto;
			background-color:rgba(11, 79, 108,1);
			float:left;
			margin-top:5vw;
			margin-left:5vw;
			color:white;
			border-radius:3vw;
			font-size:3vw;
		}
		
		.Contador_azul-icone{
			width:24vw;
			height:36vw;
			background-color:rgba(255,255,255,0);
			float:left;
			background-image:url("../assets/img/loading-process-branco.svg");
			background-repeat:no-repeat;
			background-position:center center;
			background-size:24vw auto;
			margin-left:3vw;
		}
		.Contador_azul-icone-txt{
			width:11.4vw;
			height:11.4vw;
			background-color:rgba(255,255,255,0);
			float:left;
			margin-left:6vw;
			margin-top:12vw;
			font-size:2.1vw;
			border-radius:15vw;
			line-height:3.3vw;
		}
		.Contador_azul-icone-txt span{
			font-size:3vw;
			line-height:3.6vw;
			font-weight:bold;
		}
		.Contador_azul-txt span{
			color:red;
			font-weight:bold;
		}
		.Contador_azul-trajeto{
			width:60vw;
			height:17vw;
			line-height:5vw;
			background-color:rgba(255,255,255,0);
			float:left;
			text-align:left;
			color:rgb(250,250,260);
			padding-top:3vw;
			padding-left:3vw;
			font-size:3.5vw;
		}
		.Contador_azul-txt{
			width:60vw;
			height:12vw;
			line-height:5vw;
			background-color:rgba(255,255,255,0);
			float:left;
			text-align:left;
			color:rgb(250,250,260);
			padding-top:3vw;
			padding-left:3vw;
			font-size:3.5vw;
		}
		.Contador_azul-marcador{
			position:absolute;
			width:17.1vw;
			height:0.6vw;
			background-color:rgba(11, 79, 108,1);
			margin-left:18vw;
		}
		.Trajeto-bloco-inicio{
			width:12vw;
			height:15vw;
			background-color:rgba(255,0,0,0);
			float:left;
			margin-top:0vw;
			margin-left:1.5vw;
			margin-right:2.4vw;
		}
		.Trajeto-bloco{
			width:13.5vw;
			height:15vw;
			background-color:rgba(255,0,0,0);
			float:left;
			margin-top:0vw;
		}
		.Trajeto-icone{
			width:100%;
			height:6vw;
			background-color:rgba(255,0,0,0);
			float:left;
			background-repeat:no-repeat;
			background-position:center center;
			background-size:auto 3.9vw;
		}
		.bloco-01 .Trajeto-icone{
			background-image:url("../assets/img/empty-drawer.svg");
		}
		.bloco-02 .Trajeto-icone{
			background-image:url("../assets/img/stopwatch.svg");
		}
		.bloco-03 .Trajeto-icone{
			background-image:url("../assets/img/car.svg");
		}
		.bloco-04 .Trajeto-icone{
			background-image:url("../assets/img/checked.svg");
		}
		.bloco-01.concluido .Trajeto-icone{
			background-image:url("../assets/img/empty-drawer-red.svg");
		}
		.bloco-02.concluido .Trajeto-icone{
			background-image:url("../assets/img/stopwatch-red.svg");
		}
		.bloco-03.concluido .Trajeto-icone{
			background-image:url("../assets/img/car-red.svg");
		}
		.bloco-04.concluido .Trajeto-icone{
			background-image:url("../assets/img/checked-red.svg");
		}
		.Trajeto-marcador{
			width:0.9vw;
			height:0.9vw;
			background-color:rgba(255,255,255,1);
			border:1vw solid rgb(204,204,214);
			border-radius:15vw;
			display: inline-block;
			position:relative;
			z-index:1;
			margin-left: 5vw;
		}
		.Trajeto-bloco-inicio.concluido .Trajeto-marcador,
		.Trajeto-bloco.concluido .Trajeto-marcador{
			border:0.6vw solid rgb(230, 59, 79);
		}
		.Trajeto-bloco.concluido .Trajeto-linha{
			background-color:rgb(230, 59, 79);
		}
		.Trajeto-linha{
			width:12vw;
			height:0.6vw;
			background-color:rgb(204,204,214);
			position:absolute;
			margin-top:8.1vw;
			margin-left:-7vw;
			z-index:0;
		}
		.Trajeto-txt{
			width:100%;
			height:auto;
			background-color:rgba(255,0,0,0);
			float:left;
			font-size:1.8vw;
			line-height:2.4vw;
			text-align:center;
			color:white;
		}
	
	}


</style>