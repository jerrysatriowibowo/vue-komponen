<template>
    <div>
        <input type="text" v-model="cari" placeholder="Cari Data">
        <ul>
            <li v-for="item in cariData" :key="item.id">{{ item.title }} - {{ item.price }}</li>
        </ul>
        <p v-if="cariData.length === 0">Tidak Ada Data Ditemukan</p>
    </div>
</template>
<script>
export default {
    data(){
        return {
            cari: '',
            product: []
        }
    },
    created() {
            this.product = [
                {id: 1, title: "Baju", price: 250000},
                {id: 2, title: "Sepatu", price: 150000},
                {id: 3, title: "Celana", price: 175000},
                {id: 4, title: "Topi", price: 25000},
                {id: 5, title: "Sendal", price: 15000}
            ]
        },
        computed: {
            cariData() {
                return this.product.filter((item) => {
                    return item.title.match(this.cari)
                });
            }
        }
    }
</script>