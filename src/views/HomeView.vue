<template>
  <div class="container">
    <Header/>
    <FirstBlock/>
    <div class="medium-grid">
      <MediumPhotoBlock image="https://pbs.twimg.com/media/FbB_qYbaQAAXAVF?format=jpg&name=large" title="Photography" description="Helmut Lang celebrates taxi drivers worldwide in latest campaign" author="By Alessandra Ortiz"/>
      <MediumPhotoBlock image="https://uploads-ssl.webflow.com/5c718ab52d05cea42c971e40/5c718ab52d05ce6e50971ebb_image-13-p-1600.jpeg" title="Photography" description="Helmut Lang celebrates taxi drivers worldwide in latest campaign" author="By Alessandra Ortiz"/>
      <MediumPhotoBlock image="https://mir-s3-cdn-cf.behance.net/project_modules/1400/54b8e853982217.5948f0862456c.jpg" title="Photography" description="Helmut Lang celebrates taxi drivers worldwide in latest campaign" author="By Alessandra Ortiz"/>
      <MediumPhotoBlock image="" title="Photography" description="Helmut Lang celebrates taxi drivers worldwide in latest campaign" author="By Alessandra Ortiz"/>
      <MediumPhotoBlock image="" title="Photography" description="Helmut Lang celebrates taxi drivers worldwide in latest campaign" author="By Alessandra Ortiz"/>
      <MediumPhotoBlock image="" title="Photography" description="Helmut Lang celebrates taxi drivers worldwide in latest campaign" author="By Alessandra Ortiz"/>
    </div>
    <div class="small-grid">
      <SmallPhotoBlock image="" title="" description="" author=""/>
      <SmallPhotoBlock image="" title="" description="" author=""/>
      <SmallPhotoBlock image="" title="" description="" author=""/>
      <SmallPhotoBlock image="" title="" description="" author=""/>
      <SmallPhotoBlock image="" title="" description="" author=""/>
      <SmallPhotoBlock image="" title="" description="" author=""/>
      <SmallPhotoBlock image="" title="" description="" author=""/>
      <SmallPhotoBlock image="" title="" description="" author=""/>
    </div>
    <a href="#"> <button class="button">view all latest posts</button></a>
    <div class="big-grid">
      <BigPhotoBlock image="" title="" description="" author=""/>
      <BigPhotoBlock image="" title="" description="" author=""/>
      <BigPhotoBlock image="" title="" description="" author=""/>
      <BigPhotoBlock image="" title="" description="" author=""/>
    </div>
    <!-- <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/> -->
    <Footer />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'; //@ is an alias to /src
import Header from '@/components/TheHeader.vue'; 
import Footer from '@/components/TheFooter.vue';
import MediumPhotoBlock from '@/components/MediumPhotoBlock.vue';
import SmallPhotoBlock from '@/components/SmallPhotoBlock.vue';
import BigPhotoBlock from '@/components/BigPhotoBlock.vue';
import FirstBlock from '@/components/FirstBlock.vue';

export default defineComponent({
  name: 'HomeView',
  components: {
    Header : Header,
    Footer : Footer,
    MediumPhotoBlock : MediumPhotoBlock,
    SmallPhotoBlock : SmallPhotoBlock,
    BigPhotoBlock : BigPhotoBlock,
    FirstBlock : FirstBlock,
  },
});
</script>
<style scoped lang="scss">

.button {
  border: 1px solid black;
  background-color: white;
  padding: 16px 20px;
  font-size: 15px;
  text-transform: uppercase;
  margin: 20px 0;
}
.button:hover {
  transition: .5s;
  background-color: black;
  color: white;
}
.small-grid,
.medium-grid,
.big-grid {
  width: 80%;
  row-gap: 20px;
  margin: 0 10%;
  display: grid;
  grid-template-rows: 1fr 1fr;
}
.medium-grid {
    grid-template-columns: 1fr 1fr 1fr;
  }
  .small-grid {
    grid-template-columns: 1fr 1fr 1fr 1fr;
  }
  .big-grid {
    grid-template-columns: 1fr 1fr;
    margin-bottom: 30px;
  }
</style>