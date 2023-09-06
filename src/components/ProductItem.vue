<script setup>
import ProductItemImg from '@/components/ProductItemImg.vue'
import ProductItemName from '@/components/ProductItemName.vue'
import ProductItemPrice from '@/components/ProductItemPrice.vue'

defineProps({
  item: {
    type: Object,
  }
})
</script>

<template>
  <ProductItemImg />
  <ProductItemName />
  <ProductItemPrice />
</template>

<style scoped>


</style>
