<script setup>
import { onMounted } from 'vue';
import { Viewer } from 'cesium';

onMounted(()=>{
  const viewer = new Viewer('cesiumContainer');
})
</script>

<template>
  <div id="cesiumContainer"></div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
html,body,#cesiumContainer{
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
  overflow: hidden;
}
</style>
