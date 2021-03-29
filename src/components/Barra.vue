<template>

	<div class="barra">

		<div class="barra-img"></div>
		
	</div>

</template>

<script>
export default {

	name: 'Barra',

}
</script>

<style scoped>

	.barra{
		width:5vw;
		height:100vh;
		background-color:rgb(230, 59, 79);
		float:left;
	}
	.barra-img{
		width:4vw;
		height:4vw;
		background-color:rgba(255,0,0,0);
		background-image:url( "../assets/img/logo.png" );
		background-repeat:no-repeat;
		background-position:center center;
		background-size:100% auto;
		margin:0 auto;
		margin-top:1vw;
	}
	
	@media only screen and (max-width:1279px){
	
		.barra{
			width:100vw;
			height:20vw;
		}
		.barra-img{
			width:16vw;
			height:16vw;
			margin-top:2vw;
			margin-left:2vw;
			float:left;
		}
	
	}


</style>