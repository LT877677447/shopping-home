<script setup>
import ProductItem from '../components/ProductItem.vue';

const item = {
  imgSrc: '/img/naifen.jpg',
  price: 110.5,
  name: '飞鹤奶粉'
}
const config = {}
const productList = new Array(40).fill(item)

</script>
<template>
  <div>
    <ul class="product-list">
      <ProductItem
        v-for="(item, idx) of productList"
        :item="item"
        :config="config"
      />
    </ul>
  </div>
</template>

<style lang="less" scoped>
* {
  padding: 0;
  margin: 0;
}
.product-list {
  &::after {
    content: '';
    clear: both;
    display: block;
  }
}
</style>
