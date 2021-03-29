<template>

	<div id="app">

		<Barra/>
		<Usuario/>
		<Mapa/>
		<Painel_mobile/>

	</div>

</template>

<script>

	import Barra from './components/Barra.vue'
	import Usuario from './components/Usuario.vue'
	import Mapa from './components/Mapa.vue'
	import Painel_mobile from './components/Painel_mobile.vue'

	export default {

		name: 'App',

		components: {

			Barra,
			Usuario,
			Mapa,
			Painel_mobile,

		}

	}

</script>

<style>

	body{
		margin:0;
		padding:0;
		background-color:rgba(230,230,240,1);
	}
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin:0;
		padding:0;
	}

</style>
