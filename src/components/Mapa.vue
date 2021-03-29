<template>
	<div>
	
		<MglMap
			:accessToken="accessToken"
			:mapStyle.sync="mapStyle"
			:center="coordinates"
			:zoom="zoom"
			class="mapa"
		>
		
			<MglMarker :coordinates="coordinates" color="blue" />
			<MglAttributionControl />
			<MglScaleControl position="bottom-right" />
			<MglNavigationControl position="bottom-right" />
			<MglGeolocateControl position="bottom-right" />
			
			<Painel />
		
		</MglMap>
	
	</div>

</template>

<script>
import 'mapbox-gl/dist/mapbox-gl.css';
import Mapbox from "mapbox-gl";
import Painel from './Painel.vue';

import {
	MglMap,
    MglMarker,
	MglAttributionControl,
	MglNavigationControl,
	MglGeolocateControl,
	MglScaleControl
} from "vue-mapbox";


export default {

	name: 'Mapa',

	components: {
		MglMap,
		MglMarker,
		MglAttributionControl,
		MglNavigationControl,
		MglGeolocateControl,
		MglScaleControl,
		Painel
	},

	data() {
		return {
			accessToken: 'pk.eyJ1IjoiY2Fpb2xvdXJlaXJvIiwiYSI6ImNrbXRrYmtnZjBkcGkyb3BjZHJjZjBtOTQifQ.5K3EaPM8Z80g1ciyYO8uCA',
			mapStyle: 'mapbox://styles/mapbox/streets-v11',
			coordinates: [-46.636, -23.547],
			zoom:9
		};
	},

	created() {
		this.mapbox = Mapbox;
	}

}
</script>

<style scoped>

	.mapa{
		float:left;
		width:93vw;
		height:40vw;
		margin-top:3vw;
		margin-left:1vw;
		background-color:rgba(0,0,0,0.8);
		padding:0vw;
	}
	
	@media only screen and (max-width:1279px){
	
		.mapa{
			width:99vw;
			height:150vw;
			margin-top:3vw;
		}
		
	}

</style>