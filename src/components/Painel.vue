<template>

	<div class="Painel">

		<Central_ajuda/>
		<Trajeto/>
		<Status/>
		<Endereco_entrega/>
		<Horario_estimado/>
		<Contador_branco/>
		<Historico/>
		
	</div>

</template>

<script>
import Central_ajuda from './Central_ajuda.vue';
import Trajeto from './Trajeto.vue';
import Status from './Status.vue';
import Endereco_entrega from './Endereco_entrega.vue';
import Horario_estimado from './Horario_estimado.vue';
import Contador_branco from './Contador_branco.vue';
import Historico from './Historico.vue';

export default {

	name: 'Painel',
	
	components: {
		Central_ajuda,
		Trajeto,
		Status,
		Endereco_entrega,
		Horario_estimado,
		Contador_branco,
		Historico,
	},

}
</script>

<style scoped>

	*{
	scrollbar-width: thin;
		scrollbar-color: rgb(235, 235, 245) rgb(255, 255, 255);
	}
	::-webkit-scrollbar{
		background-color:rgb(255, 255, 255);
	}
	::-webkit-scrollbar-thumb{
		background-color:rgb(235, 235, 245);
	}

	.Painel{
		width:20vw;
		height:38vw;
		background-color:rgba(255,255,255,1);
		float:left;
		position:relative;
		margin-top:1vw;
		margin-left:0.5vw;
		box-shadow:0.3vw 0.1vw 0.5vw rgba(0,0,0,0.2);
		overflow:auto;
	}
	
	@media only screen and (max-width:1279px){
	
		.Painel{
			display:none;
		}
	
	}


</style>