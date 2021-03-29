<template>

	<div class="Status">

		<div class="Status-titulo">Saiu para entrega</div>
		<div class="Status-txt">Seu pedido da <strong>Dafiti</strong> saiu para entrega, e será <strong>entregue</strong> no <strong>endereço</strong>:</div>
		
	</div>

</template>

<script>
export default {

	name: 'Status',

}
</script>

<style scoped>

	.Status{
		width:17.7vw;
		height:auto;
		background-color:rgba(11, 79, 108,1);
		float:left;
		margin-left:1vw;
		color:white;
		border-radius:0.5vw;
		font-size:0.95vw;
		padding-bottom:0.5vw;
	}
	
	.Status-titulo{
		width:94%;
		height:auto;
		background-color:rgba(255,0,0,0);
		float:left;
		text-transform:uppercase;
		line-height:2vw;
		margin-top:0.5vw;
		text-align:left;
		padding-left:3%;
		padding-right:3%;
		font-weight:bold;
	}

	.Status-txt{
		width:96%;
		height:auto;
		background-color:rgba(255,0,0,0);
		float:left;
		text-align:left;
		padding-left:3%;
		padding-right:1%;
		font-size:0.8vw;
		padding-bottom:0.5vw;
	}
	
	@media only screen and (max-width:1279px){
	
		.Status{
		}
	
	}


</style>