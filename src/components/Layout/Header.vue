<template>
    <header class="header">
        <div class="header-top">
            <div class="header-top-search">
                <img src="../svg/Search.svg">
            </div>
            <a href="#" class="header-logo">Text.ru</a>
            <div class="header-top-right">
                <div class="header-top-right_cart">
                    <a href="#">
                    <img src="../svg/Shopping--cart.svg">
                </a>
                </div>
                <div class="header-top-right_profile">
                    <a href="#">
                    <img src="../svg/User.svg">
                </a>
                </div>
            </div>
        </div>
        <div class="header-menu">
            <a
            class="header-menu_link"
             :href="element.path" 
             v-for="(element,i) of menu"
             :key="i">{{element.name}}</a>
        </div>
    </header>
</template>
<script setup>
import {ref} from 'vue'
const menu = [
    {
        name:'Биржа контента',
        path:'/birja'
    },
    {
        name:'Проверка уникальности',
        path:'/proverka'
    },
    {
        name:'Анализ текста',
        path:'/analis'
    },
    {
        name:'Тарифы',
        path:'/analis'
    },
    {
        name:'Поддержка',
        path:'/analis'
    },
    {
        name:'Новости',
        path:'/analis'
    }
]
</script>
<style lang="scss" scoped>
.header{
    background: #fff;
    height: 132px;
    &-top{
        display:grid;
    grid-template-columns: repeat(3, 1fr);
        justify-content: space-between;
        height: 70px;
        align-items: center;
        border-bottom: 1px solid rgba(0,0,0,.1);
       //   margin: 0 28px;
        &-right {
        display:flex;
        align-items: center;
        justify-content:flex-end ;
        &_cart{
            margin-right: 16px;
        }
    }
    }
    &-logo{
        font-family: Arial, Helvetica, sans-serif;
        font-size: 24px;
        color:#22202E;
        text-decoration: none;
        text-align: center;
        &-hover{
            text-decoration: underline;
        }
    }
 &-menu{
    height: 62px;
    display:flex;
    justify-content:center;
    align-items: center;
    &_link{
        margin:0 22px;
        color: #726E8D;
        text-decoration:none;
        &:hover{
            text-decoration: underline;
        }
    }
 }
}
</style>