<template>

	<div class="usuario">Fulano de Tal da Silva</div>

</template>

<script>
export default {

	name: 'Barra',

}
</script>

<style scoped>

	.usuario{
		width:auto;
		height:auto;
		line-height:1.2vw;
		text-align:left;
		background-color:rgba(230, 59, 79,0);
		color:rgba(230, 59, 79,1);
		float:right;
		margin-top:1vw;
		margin-right:1vw;
		padding:0.5vw;
		border-left:0.3vw solid rgb(230, 59, 79);
		text-transform:uppercase;
		font-size:1vw;
		font-weight:bold;
	}
	
	@media only screen and (max-width:1279px){
	
		.usuario{
			display:none;
		}
	
	}


</style>