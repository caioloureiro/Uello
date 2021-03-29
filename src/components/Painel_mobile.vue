<template>

	<div class="Painel_mobile">

		<Contador_azul/>
		<Central_ajuda/>
		<Status/>
		<Endereco_entrega/>
		
	</div>

</template>

<script>
import Contador_azul from './Contador_azul.vue';
import Central_ajuda from './Central_ajuda.vue';
import Status from './Status.vue';
import Endereco_entrega from './Endereco_entrega.vue';

export default {

	name: 'Painel_mobile',
	
	components: {
		Contador_azul,
		Central_ajuda,
		Status,
		Endereco_entrega,
	},

}
</script>

<style scoped>

	.Painel_mobile{
		display:none;
	}
	
	@media only screen and (max-width:1279px){
	
		.Painel_mobile{
			width:100vw;
			height:155vw;
			background-color:rgba(255,0,0,0);
			position:absolute;
			margin-top:20vw;
			display:block;
			z-index:3;
			overflow-y:auto;
			overflow-x:none;
		}
	
	}


</style>