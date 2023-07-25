<template>
  <div>
    <h1>Belajar Vue.JS</h1>
    <NewComponent></NewComponent>
    <WatchersComponent nama="Jerry" umur="19"></WatchersComponent>
  </div>
</template>
<script setup>
import NewComponent from './components/NewComponent.vue';
import WatchersComponent from './components/WatchersComponent.vue';
</script>