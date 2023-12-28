<template>
    <div class="about-brand">
        <h3 class="about-brand_title">Сервис проверки текста на уникальность и<a  class="about-brandd_title_red"> биржа копирайтинга</a></h3>      
   <div class="about-brand-elements">
    <div 
    class="about-brand-element"
    v-for="(element,i) of aboutBrands"
   :key="i">
        <img 
        :src="element.img" 
        :alt="element.title"
        class="about-brand-element_img">
        <h4 class="about-brand-element_title">{{ element.title }}</h4>
        <span class="about-brand-element_description">{{ element.description }}</span>
    </div>
   </div>
   </div>
</template>
<script setup>
import {ref} from 'vue'
const aboutBrands = [
    {
        img:'src/components/svg/изображение_2023-12-28_050425534 1 (2).svg',
        title: 'Проверить текст',
        description:'На уникальность, орфографию, заспамленность'
    },
    {
        img:'src/components/svg/image.svg',
        title: 'Заказать текст',
        description:'Текстовый контент под любые задачи'
    },
    {
        img:'src/components/svg/image1.svg',
        title: 'Работать автором',
        description:'Зарабатывайте на любимом деле'
    },
    {
        img:'src/components/svg/robot.svg',
        title: 'Нейросеть для текстов',
        description:'Проверяйте, создавайте и редактируйте'
    }
]
</script>




<style lang="scss" scoped>
.about-brand{
    padding:10px 0 100px 0;
    &_title{
        text-align: center;
        font-size:24px;
        color:#000000;
        margin: 0 0 84 0;
        &_red{
            color:#a00c0c;    
        }      
    }
    &-elements{
        
            display: grid;
       grid-template-columns: repeat(4,250px);
      justify-content:space-between;
  
     }
    &-element{
            color:#2A254B;
            background-color:#ffffff;
            border-radius: 20px;
       
            &_img{
                    display:block;
                    margin-bottom: 12px;
            }
            &_title{
                margin:0 0 12px 0;
          
            font-size: 20px;
            }
            &_description{
                font-size: 16px;
                line-height:1.5 ;
            }
    }
}
</style>