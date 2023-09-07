<script setup>
defineProps({
  name: {
    type: String,
    default: ''
  }
})
</script>

<template>
  <div class="product-item-name">
    {{ name }}
  </div>
</template>

<style lang="less" scoped>

</style>
