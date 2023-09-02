<template>
  <div id="cesiumContainer">
  </div>
</template>

<script setup>
import * as Cesium from 'cesium'
import { onMounted } from 'vue'

onMounted(() => {
  Cesium.Ion.defaultAccessToken = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJqdGkiOiIyNjAzZTE3OS1lNzVmLTQ3NmUtODQyMC02MTdiOTIwYzBiOWYiLCJpZCI6MTY0MDMwLCJpYXQiOjE2OTM2MzY1NjZ9.9O-QAxJzRmI2LsaBAct4Qud1ITKzaY5fLFNp2MNt-0Y'
  new Cesium.Viewer('cesiumContainer')

})

</script>

<style scoped>
#cesiumContainer {
  width: 100vw;
  height: 100vh;
}
</style>
