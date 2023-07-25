<template>
    <div>
      <MyComponent 
        :nama="nama" 
        :umur="umur"
        @greeted="onGreeted"></MyComponent>
    </div>
  </template>
  <script>
  import MyComponent from './MyComponent.vue';
  export default {
    components: {
      MyComponent
    },
    data() {
    return {
      nama: 'Bimoli',
      umur: 35
      };
    },
    methods: {
      onGreeted() {
        console.log('Kamu udah disapa, bro!');
      }
    }
  }
  </script>