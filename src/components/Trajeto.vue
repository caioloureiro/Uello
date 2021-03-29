<template>

	<div class="Trajeto">

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

</template>

<script>
export default {

	name: 'Trajeto',

}
</script>

<style scoped>

	.Trajeto{
		width:100%;
		height:9.1vw;
		background-color:rgba(255, 255, 255,1);
		float:left;
	}
	.Trajeto-bloco-inicio{
		width:3vw;
		height:5vw;
		background-color:rgba(255,0,0,0);
		float:left;
		margin-top:2vw;
		margin-left:0.5vw;
		margin-right:0.8vw;
	}
	.Trajeto-bloco{
		width:4.5vw;
		height:5vw;
		background-color:rgba(255,0,0,0);
		float:left;
		margin-top:2vw;
	}
	.Trajeto-icone{
		width:100%;
		height:2vw;
		background-color:rgba(255,0,0,0);
		float:left;
		background-repeat:no-repeat;
		background-position:center center;
		background-size:auto 1.3vw;
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
		width:0.3vw;
		height:0.3vw;
		background-color:rgba(255,0,0,0);
		border:0.2vw solid rgb(204,204,214);
		border-radius:5vw;
		display: inline-block;
		position:relative;
		z-index:1;
	}
	.Trajeto-bloco-inicio.concluido .Trajeto-marcador,
	.Trajeto-bloco.concluido .Trajeto-marcador{
		border:0.2vw solid rgb(230, 59, 79);
	}
	.Trajeto-bloco.concluido .Trajeto-linha{
		background-color:rgb(230, 59, 79);
	}
	.Trajeto-linha{
		width:4vw;
		height:0.2vw;
		background-color:rgb(204,204,214);
		position:absolute;
		margin-top:2.7vw;
		margin-left:-2vw;
		z-index:0;
	}
	.Trajeto-txt{
		width:100%;
		height:auto;
		background-color:rgba(255,0,0,0);
		float:left;
		font-size:0.6vw;
		line-height:0.8vw;
		text-align:center;
		color:rgb(51,51,61);
	}
	
	@media only screen and (max-width:1279px){
	
		.Trajeto{
		}
	
	}


</style>