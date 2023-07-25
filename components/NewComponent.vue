<template>
    <div>
        <MyComponent nama="Jerry" umur="19" alamat="Sukamenak Indah"></MyComponent>
        <TesComponent name="Cuki" usia="19"></TesComponent>
        <Tes2Component></Tes2Component>
        <FooterComponent></FooterComponent>
        <EventComponent></EventComponent>
        </div>
</template>
<script setup>
import MyComponent from './MyComponent.vue';
import FooterComponent from './FooterComponent.vue';
import TesComponent from './TesComponent.vue';
import Tes2Component from './Tes2Component.vue';
import EventComponent from './EventComponent.vue';
</script>