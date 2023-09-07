<script setup>
defineProps({
  price: {
    type: [String, Number],
    default: '',
  }
})
</script>

<template>
  <div class="product-item-price">
    {{ price }}
  </div>
</template>

<style lang="less" scoped>


</style>
