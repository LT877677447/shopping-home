<script setup>
import ProductItemImg from '@/components/ProductItemImg.vue'
import ProductItemName from '@/components/ProductItemName.vue'
import ProductItemPrice from '@/components/ProductItemPrice.vue'

defineProps({
  item: {
    type: Object,
  },
  config: {
    type: Object,
  },
})

</script>

<template>
  <li class="product-list-item">
    <a href="">
      <ProductItemImg :img-src="item.imgSrc" />
      <ProductItemName :name="item.name" />
      <ProductItemPrice :price="item.price" />
    </a>
  </li>
</template>

<style scoped lang="less">
.product-list-item {
  list-style: none;
  width: 190px;
  height: 266px;
  margin: 0 5px 8px;
  float: left;
  a {
    width: 100%;
    height: 100%;
    display: inline-block;
  }
}
</style>
