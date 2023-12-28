<script setup>
//import {ref} from 'vue'
import Header from './components/Layout/Header.vue'
import AboutBrand from './components/Layout/AboutBrand.vue'
import Products4Column from './components/Products4Columns.vue'
import Part4 from './components/Layout/Part4.vue'
import Footer from './components/Layout/Footer.vue'

</script>

<template>
  <div class="container">
  <Header></Header>
  <AboutBrand></AboutBrand>
  <Products4Column 
>
</Products4Column>
<Part4></Part4>
<Footer></Footer>
  </div>

</template>

<style lang="scss" >
@import url('https://fonts.cdnfonts.com/css/satoshi');
*{
  box-sizing: border-box;
}
body{
  background-color: #d6e8f2;

background-image: url(images/gradient.jpg);

background-repeat: repeat-x;
  font-size: 16px;
  margin:0;
  padding: 0;
  font-family: 'Satoshi', sans-serif;
}
.container{    
 max-width: 1490px;
 margin: auto;
}
</style>
