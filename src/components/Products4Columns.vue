<template>
    <div class="products">
        <Products v-for="product of products" 
  :key="product.id"
  :img="product.img"
  :title="product.title"
  :price="product.price"></Products>
    </div>
  
</template>
<script setup>
import Products from '../components/Products.vue'
import {ref} from 'vue'
const products = ref ([
  {
    id:1,
    img:'src/components/svg/Без имени.png',
    title:'Проверка уникальности Вашего сайта',
    price: 250
  },
  {
    id:2,
    img:'src/components/svg/Без имени.png',
    title:'Проверка уникальности документа',
    price: 100
  },
  {
    id:3,
    img:'src/components/svg/Без имени.png',
    title:'Настройка всего текстового контента',
    price: 1000
  },
  {
    id:4,
    img:'src/components/svg/Без имени.png',
    title:'Проверка орфографии',
    price: 100
  }

])

</script>
<style lang="scss" scoped>
.products{
    padding: 0 80px;
    display: flex;
    grid-template-columns: repeat(4,1fr);
    column-gap:20px;
}
</style>