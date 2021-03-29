<template>

	<div class="Historico">
	
		<div class="Historico-titulo">
		
			<div class="Historico-icone">

				<svg
					version="1.1"
					id="Capa_1"
					xmlns="http://www.w3.org/2000/svg"
					xmlns:xlink="http://www.w3.org/1999/xlink"
					x="0px"
					y="0px"
					viewBox="0 0 448 448"
					style="enable-background:new 0 0 448 448;"
					xml:space="preserve"
					fill="rgb(230, 59, 79)"
				>
					<g>
						<g>
							<g>
								<polygon points="234.667,138.667 234.667,245.333 325.973,299.52 341.333,273.6 266.667,229.333 266.667,138.667 			"/>
								<path d="M255.893,32C149.76,32,64,117.973,64,224H0l83.093,83.093l1.493,3.093L170.667,224h-64
									c0-82.453,66.88-149.333,149.333-149.333S405.333,141.547,405.333,224S338.453,373.333,256,373.333
									c-41.28,0-78.507-16.853-105.493-43.84L120.32,359.68C154.987,394.453,202.88,416,255.893,416C362.027,416,448,330.027,448,224
									S362.027,32,255.893,32z"/>
							</g>
						</g>
					</g>
				</svg>
			
			</div>Histórico
		
		</div>
		
		<div class="Historico-item">
		
			<div class="">
				<div class="Historico-item-mark"></div>
				<div class="Historico-item-sutitulo">Solicitação recebida</div>
				<div class="Historico-item-down"></div>
				<div class="Historico-item-txt">14/05 - 22h41</div>
			</div>
		
		</div>
		
		<div class="Historico-item">
		
			<div class="">
				<div class="Historico-item-mark"></div>
				<div class="Historico-item-sutitulo">Solicitação recebida</div>
				<div class="Historico-item-down"></div>
				<div class="Historico-item-txt">14/05 - 22h41</div>
			</div>
		
		</div>
		
		<div class="Historico-item Historico-final">
		
			<div class="">
				<div class="Historico-item-mark"></div>
				<div class="Historico-item-sutitulo">Solicitação recebida</div>
				<div class="Historico-item-down"></div>
				<div class="Historico-item-txt">14/05 - 22h41</div>
			</div>
		
		</div>
	
	</div>

</template>

<script>
export default {

	name: 'Historico',

}
</script>

<style scoped>

	.Historico{
		width:17.7vw;
		height:auto;
		background-color:rgba(11, 79, 108,0);
		float:left;
		margin-left:1vw;
		color:rgb(230, 59, 79);
		border-radius:0.5vw;
		font-size:0.95vw;
		padding-bottom:0.5vw;
		border:0.1vw solid rgb(230, 59, 79);
		margin-bottom:2vw;
	}
	.Historico-icone{
		width:1vw;
		height:1vw;
		float:left;
		margin-top:0.1vw;
		margin-left:2vw;
		margin-right:0.5vw;
	}
	.Historico-titulo{
		width:100%;
		height:auto;
		background-color:rgba(255,0,0,0);
		float:left;
		text-align:left;
		line-height:3vw;
		font-size:1.2vw;
	}
	.Historico-item{
		width:100%;
		height:auto;
		background-color:rgba(255,0,0,0);
		float:left;
	}
	.Historico-item-mark{
		width:1.6vw;
		height:1.6vw;
		background-color:rgba(255,0,0,0);
		float:left;
		border-radius:5vw;
		margin-left:0.9vw;
		margin-right:0.6vw;
		border:0.2vw solid rgb(230, 59, 79);
	}
	.Historico-item-sutitulo{
		width:13.7vw;
		height:2vw;
		line-height:2vw;
		background-color:rgba(255,0,0,0);
		float:left;
		color:rgb(150,150,160);
		text-align:left;
	}
	.Historico-item-down{
		width:0.2vw;
		height:2.3vw;
		background-color:rgb(230, 59, 79);
		float:left;
		margin-left:1.75vw;
		margin-right:1.5vw;
		margin-top:-0.2vw;
	}
	.Historico-item-txt{
		width:13.7vw;
		height:2vw;
		line-height:2vw;
		background-color:rgba(255,0,0,0);
		float:left;
		color:rgb(150,150,160);
		text-align:left;
	}
	.Historico-final .Historico-item-down{
		background-color:rgba(230, 59, 79,0);
	}
	@media only screen and (max-width:1279px){
	
		.Historico{
		}
	
	}


</style>