<template>
    <div v-if="usia > 18">
        <p>Selamat Datang {{ name }}</p>
    </div>
    <div v-else>
        <p>Maaf Kamu Belum Cukup Umur</p>
    </div>
    <button @click="greet">Say Hello</button>
</template>
<script>
export default {
    props: ['name', 'usia'],
    methods: {
        greet(){
            alert("Hallo " + this.name)
            alert("Usia " + this.usia)
        }
    }
}
</script>