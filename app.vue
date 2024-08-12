<script setup>
import { onMounted, ref } from "vue";
import mapboxgl from "mapbox-gl";
import "mapbox-gl/dist/mapbox-gl.css";
import style from "./mapbox/style.json";

mapboxgl.accessToken = "";

const mapContainer = ref();

onMounted(() => {
  new mapboxgl.Map({
    "container": mapContainer.value,
    "style": style
  });
});
</script>

<template>
  <div class="container">
    <div class="content">
      <div ref="mapContainer" class="map"></div>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-flow: column;
  height: 100%;
}

.content {
  flex-grow: 1;
  position: relative
}

.map {
  height: 100%;
}
</style>