<template>
    <div class="row">
        <flNavBar />
        <div id="map" class="col-md-12 map">

        </div>
    </div>
</template>

<script>
import {LMap, LTileLayer, LMarker} from 'vue2-leaflet'
import flNavBar from './components/navbar/main.vue'

export default {
  name: 'app',
  components: {
    flNavBar
  },

  mounted() {
    this.getMapa()
  },

  methods: {
    getMapa(){
      zoomControl: false
      attributionControl: false

        var map = L.map('map').setView([51.505, -0.09], 13);

        L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png').addTo(map);

        L.marker([51.5, -0.09]).addTo(map)
            .bindPopup('A pretty CSS3 popup.<br> Easily customizable.')
            .openPopup();
    }
  }
}
</script>

<style>
.row{
  margin: 0px !important;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #ffffff;
}
#map.col-md-12.map.leaflet-container.leaflet-touch.leaflet-fade-anim.leaflet-grab.leaflet-touch-drag.leaflet-touch-zoom {
    margin: 0 !important;
    width: 100% !important;
    height: 100% !important;
    min-height: 900px !important;
}

@media (max-width: 620px){
    
}

</style>
