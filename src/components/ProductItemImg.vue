<script setup>
import { reactive, computed } from 'vue'
const props = defineProps({
  imgSrc: {
    type: String,
    default: ''
  }
})

</script>

<template>
  <div class="product-item-img">
    <img :src="imgSrc" >
  </div>
</template>

<style scoped lang="less">
.product-item-img {
  width: 190px;
  height: 190px;
  img {
    width: 100%;
    height: 100%;
  }
}
</style>
