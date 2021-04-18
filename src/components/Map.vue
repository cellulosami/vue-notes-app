<template>
  <div id="map">map
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
  </div>
</template>

<script>
	// TO MAKE THE MAP APPEAR YOU MUST
	// ADD YOUR ACCESS TOKEN FROM
	// https://account.mapbox.com


export default {
  mounted: function () {
    mapboxgl.accessToken = 'pk.eyJ1IjoiY2VsbHVsb3NhbWkiLCJhIjoiY2tubmZtY2xxMHk4YTJvbHRkeWtzc3E1ZCJ9.CXdc1u728zLWf4422wIITQ';
    var map = new mapboxgl.Map({
      container: 'map', // container id
      style: 'mapbox://styles/mapbox/streets-v11', // style URL
      center: [-74.5, 40], // starting position [lng, lat]
      zoom: 9 // starting zoom
    });
  }
}
</script>

<style>
body { 
  margin: 100; 
  padding: 100; 
}

#map { 
  position: absolute; 
  top: 0; 
  bottom: 1000; 
  width: 100%; 
}
</style