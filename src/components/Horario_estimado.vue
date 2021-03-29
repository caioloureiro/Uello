<template>

	<div class="Horario_estimado">Horário estimado: 14:45 - 16:58</div>

</template>

<script>
export default {

	name: 'Horario_estimado',

}
</script>

<style scoped>

	.Horario_estimado{
		width:17.7vw;
		height:3vw;
		line-height:3vw;
		background-color:rgba(255, 0, 0,0);
		float:left;
		margin-left:1vw;
		font-size:0.85vw;
		padding-bottom:0.5vw;
		color:rgba(11, 79, 108,1);
		text-transform:uppercase;
		font-weight:bold;
	}
	
	.Horario_estimado:before{
		content:'';
		position:relative;
		width:1vw;
		height:3vw;
		background-image:url(../assets/img/clock.svg);
		background-repeat:no-repeat;
		background-position:center center;
		background-size:auto 1vw;
		float:left;
	}
	
	@media only screen and (max-width:1279px){
	
		.Horario_estimado{
		}
	
	}


</style>