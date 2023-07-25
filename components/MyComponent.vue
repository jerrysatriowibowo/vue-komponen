<template>
    <div>
        <h2>Hallo Dunia</h2>
        <p>Nama : {{ nama }}</p>
        <p>Umur : {{ umur }}</p>
    </div>
</template>
<script>
export default {
    props: ['nama', 'umur']
}
</script>
<style>
h1{
    color: rebeccapurple;
    text-align: center;
    background-color: aqua;
}
h2{
    text-align: left;
}
p{
    color: red;
}
</style>