<script setup>
import Product from './components/Product.vue';
</script>

<template>
    <main>
        <h2>Quantity {{ quantity }}</h2>
        <Product
            component-title="Prodotto"
            component-description="Descrizione del prodotto"
            price="20"
        />
    </main>
</template>


<style scoped>
</style>

