<template>
    <div class="card text-center">
        <img :src="product.image" alt="product thumb" class="thumb">
        <p class="font-bold text-grey-500 m-4 truncate">{{ product.title }}</p>
        <NuxtLink :to="`/products/${product.id}`">{{ p.title }}
            <p class="btn my-4">View Details</p>
        </NuxtLink>
    </div>
</template>

<script setup>
    const { product } = defineProps({})
</script>
<style lang="scss" scoped>

</style> 