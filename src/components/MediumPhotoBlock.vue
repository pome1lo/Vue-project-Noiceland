<template>
    <div class="MediumPhotoBlock">
        <img v-bind:src="image"/>
        <h1>{{ title }}</h1>
        <p>{{ description }}</p>
        <h6>{{ author }}</h6>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'MediumPhotoBlock',
  props: {
    author: String,
    title: String,
    description: String,
    image: String,
  },
});
</script>

<style scoped lang="scss">
    .MediumPhotoBlock {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        flex-wrap: wrap;
        margin-bottom: 30px;

        p, 
        h1, 
        h6,
        img {
            width: 90%;
            margin: 0 5%;
            padding: 7px;
            text-align: left;
        }
        h1 {
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
            font-size: 30px;
            text-align: left;;
            text-transform: uppercase;
            color: #000000;
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