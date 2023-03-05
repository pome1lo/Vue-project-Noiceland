<template>
  <Header/>
  <div class="container">
    <FirstBlock/>
    <div class="medium-grid">
      <MediumPhotoBlock image="https://pbs.twimg.com/media/FbB_qYbaQAAXAVF?format=jpg&name=large" title="Photography" description="Helmut Lang celebrates taxi drivers worldwide in latest campaign" author="By Alessandra Ortiz"/>
      <MediumPhotoBlock image="https://uploads-ssl.webflow.com/5c718ab52d05cea42c971e40/5c718ab52d05ce6e50971ebb_image-13-p-1600.jpeg" title="Photography" description="Bowlcut launch a new summer collection that pays homage to “UK legends”" author="BY Rosanna Ondricka"/>
      <MediumPhotoBlock image="https://mir-s3-cdn-cf.behance.net/project_modules/1400/54b8e853982217.5948f0862456c.jpg" title="Photography" description="Thousands of previously unseen photographs by Andy Warhol will be made public this Autumn" author="BY Annie Lueilwitz"/>
      <MediumPhotoBlock image="https://drscdn.500px.org/photo/38752230/m%3D900/v2?sig=5b02df052696718a364f501a97ff6543f1565e77c2180e5aa07bf1e412113fef" title="Interactive Design" description="London-based Yinka Ilori’s storytelling furniture" author="BY Annie Lueilwitz"/>
      <MediumPhotoBlock image="https://uploads-ssl.webflow.com/5fd47a3f9b6ceb79f5c9ac40/5feec439b7e4942c428e1ba0_daniela-torres-fpcCfuYW6wI-unsplash.jpg" title="Graphic Design" description="Anonymous Israeli art collective Broken Fingaz direct music video for U2 and Beck" author="BY Simeon Brekke"/>
      <MediumPhotoBlock image="https://p2.piqsels.com/preview/353/560/988/tunnel-lights-trees-snow.jpg" title="Architecture" description="Suzanne Saroff’s meticulously arranged photographs alter perceptions" author="BY Reta Torphy"/>
    </div>
    <div class="small-grid">
      <SmallPhotoBlock image="https://p2.piqsels.com/preview/489/476/929/mountain-ridge-snow-trees-thumbnail.jpg" title="Illustration" description="Japan House opens in mountainside to foster peak creativity." author="BY Reta Torphy"/>
      <SmallPhotoBlock image="https://pbs.twimg.com/media/FbB_qYbaQAAXAVF?format=jpg&name=large" title="Photography" description="Helmut Lang celebrates taxi drivers worldwide in latest campaign" author="BY Alessandra Ortiz"/>
      <SmallPhotoBlock image="https://uploads-ssl.webflow.com/5c718ab52d05cea42c971e40/5c718ab52d05ce6e50971ebb_image-13-p-1600.jpeg" title="Photography" description="Bowlcut launch a new summer collection that pays homage to “UK legends”" author="BY Rosanna Ondricka"/>
      <SmallPhotoBlock image="https://mir-s3-cdn-cf.behance.net/project_modules/1400/54b8e853982217.5948f0862456c.jpg" title="Photography" description="Thousands of previously unseen photographs by Andy Warhol will be made public this Autumn" author="BY Annie Lueilwitz"/>
      <SmallPhotoBlock image="https://drscdn.500px.org/photo/38752230/m%3D900/v2?sig=5b02df052696718a364f501a97ff6543f1565e77c2180e5aa07bf1e412113fef" title="Interactive Design" description="London-based Yinka Ilori’s storytelling furniture" author="BY Annie Lueilwitz"/>
      <SmallPhotoBlock image="https://uploads-ssl.webflow.com/5fd47a3f9b6ceb79f5c9ac40/5feec439b7e4942c428e1ba0_daniela-torres-fpcCfuYW6wI-unsplash.jpg" title="Graphic Design" description="Anonymous Israeli art collective Broken Fingaz direct music video for U2 and Beck" author="BY Simeon Brekke"/>
      <SmallPhotoBlock image="https://p2.piqsels.com/preview/353/560/988/tunnel-lights-trees-snow.jpg" title="Architecture" description="Suzanne Saroff’s meticulously arranged photographs alter perceptions" author="BY Reta Torphy"/>
      <SmallPhotoBlock image="https://climb-g.ru/wp-content/uploads/2021/04/joqsv0kin_a9.jpg" title="Graphic Design" description="Anu Ambasna’s playful illustrations celebrate club culture, brown bodies and perfect paunches" author="BY Leo Bartell"/>
    </div>
    <a href="#"> <button class="button" onclick="test()" >view all latest posts</button></a>
    <div class="big-grid">
      <BigPhotoBlock image="https://kabardewata.com/uploads/image/news_juli2018/soccer-100x81.jpg" title="Graphic Design" description="A Brief History of the FIFA World Cup Logo" author="BY Clem Onojeghuo"/>
      <BigPhotoBlock image="https://www.shopusa.com/blog/denmark/wp-content/uploads/2018/06/neko-tai-604243-unsplash-1024x768.jpg" title="Graphic Design" description="Need a guide to LA’s graphic design scene? Shoplifters’ new issue has got your back" author="BY Alessandra Ortiz"/>
      <BigPhotoBlock image="https://uploads-ssl.webflow.com/611a723da07d620a8cc30d5b/62c8122afe2a394a7c031c57_TMV-Intro2-p-1080.jpeg" title="Photography" description="Fred Rowson directs film for Years and Years" author="BY Coby Gottlieb"/>
      <BigPhotoBlock image="https://dprom.online/wp-content/uploads/2022/01/hubert-neufeld-GG1CwF4qdlg-unsplash-1-1-1.jpg" title="Illustration" description="M&C Saatchi and Fontsmith collaborate on font collection for House of St Barnabas" author="BY Annie Lueilwitz"/>
    </div>
    <!-- <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/> -->
  </div>
  <Footer />
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
.container {
  width: 80%;
  margin: 0 10%;
}
.button {
  border: 1px solid black;
  background-color: white;
  padding: 16px 20px;
  font-size: 15px;
  text-transform: uppercase;
  margin: 80px 0;
  font-family: 'Libre Franklin';
}
.button:hover {
  transition: .5s;
  background-color: black;
  color: white;
}
.small-grid,
.medium-grid,
.big-grid {
  row-gap: 20px;
  width: 100%;
  justify-content: space-between;
  display: grid;
  grid-template-rows: 1fr 1fr;
}
.medium-grid {
    grid-template-columns: 385px 385px 385px;
  }
  .small-grid {
    grid-template-columns: 285px 285px 285px 285px;
  }
  .big-grid {
    grid-template-columns: 590px 590px;
    margin-bottom: 30px;
  }
</style>

