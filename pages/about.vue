<script setup>
const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<template>
    <div class="container mx-auto p-10">
        <h1 class="text-xl font-bold text-center mb-5">Products</h1>
        <div v-for="product in products" :key="product.id">
            <p>{{ product.id }} - {{ product.title }}</p>
        </div>
    </div>
</template>
