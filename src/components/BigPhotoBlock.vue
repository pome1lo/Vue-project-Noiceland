<template>
    <div class="BigPhotoBlock">
        <div>
            <img v-bind:src="image"/>
        </div>
        <h1>{{ title }}</h1>
        <p>{{ description }}</p>
        <h6>{{ author }}</h6>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'BigPhotoBlock',
  props: {
    author: String,
    title: String,
    description: String,
    image: String,
  },
});
</script>

<style scoped lang="scss">
    .BigPhotoBlock {
        justify-content: center;
        margin-bottom: 30px;
        div {
            overflow: hidden; /// 
            width: 590px;
            height: 387px; 
        }
        div img {
            width: 590px;
            height: 387px; 
            object-fit: cover;
            transition: 1s; /* Время эффекта */
            display: block; /* Убираем небольшой отступ снизу */
        }
        img:hover {transform: scale(1.2);}
        
        p, h1, h6, img {
            text-align: left;
        }
        h1 {
            margin-top: 5px;
            text-transform: uppercase;
            color: #999999;
            font-size: 15px;
            font-family: 'Libre Franklin';
            font-weight: bold;
            font-weight: 400;
        }
        p {
            font-family: 'Tenor Sans';
            font-style: normal;
            font-weight: 400;
            font-size: 20px;
            text-align: left;;
            text-transform: uppercase;
            color: #000000;
            margin: 10px 0;
        }
        h6 {
            font-size: 15px;
            letter-spacing: 1px;
            text-transform: uppercase;
            color: #000000;
            font-family: 'Libre Franklin';
            font-style: normal;
            font-weight: 700;
        }
    }
</style>