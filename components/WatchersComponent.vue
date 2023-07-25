<template>
    <div>
        <button @click="greet">Tekan</button>
  </div>
</template>
<script>
export default {
  props: ['nama', 'umur'],
  methods: {
    greet() {
      console.log('Halo Kawan');
    }
  },
  watch: {
    umur(newUmur, oldUmur) {
      console.log('Umur Berubah Dari', oldUmur, 'Menjadi', newUmur);
    }
  }
}
</script>