<template>
    <!-- <h1 class="text-red-500 font-bold text-lg">This is a products page</h1> -->
    <div class="container mx-auto flex flex-col items-center p-10">
        <h1 class="text-center font-bold text-xl">Products</h1>
        <div v-for="product in products" :key="product.id">
            <p>{{ product.title }}</p>
        </div>
    </div>
</template>

<script setup lang="ts">
const products:any[] = ref(null)
// const filteredProducts = computed(() => {

// })

const getProducts = () => {
    const products:any[] = fetch('https://fakestoreapi.com/products')
        .then(res => res.json())
        .then(json => products.value = json)
}
getProducts()
</script>