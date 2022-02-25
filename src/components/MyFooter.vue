<template>
<section>
<div class="columns">
  <list :name="navigation.name" :columns="navigation.columns" class="block"/>
  <list :name="our_socials.name" :columns="our_socials.columns"/>
  <div class="logo">
    <podcaster/>
  </div>
  <list :name="usefull_links.name" :columns="usefull_links.columns"/>
  <list :name="information.name" :columns="information.columns"/>
</div>
</section>
</template>

<script>
import List from "./elements/List";
import Podcaster from "./elements/Podcaster";
export default {
  name: "MyFooter",
  components: {Podcaster, List},
  data(){
    return{
      navigation: {
        name: 'Navigation',
        columns: ['Home', 'Articles', 'Blog']
      },
      our_socials: {
        name: 'Our socials',
        columns: ['Instagram', 'Spotify', 'Facebook']
      },
      usefull_links: {
        name: 'Usefull links',
        columns: ['Privacy police', 'Terms & conditions', 'Exchange and return policy']
      },
      information: {
        name: 'Information',
        columns: ['About us', 'Contact us', 'Blogs', 'FAQ']
      }
    }
  }
}
</script>

<style scoped>
 section{
   background: #11024B;
   height: 60vh;
   display: flex;
   padding: 10px;
 }
 .columns{
   width: 100%;
   display: flex;
   justify-content: space-around;
   align-items: center;
 }
 @media screen and (max-width: 700px) {
   section{
     height: 100vh;
   }
   .columns{
     flex-wrap: wrap;
   }

   .block{
     /*margin: 20px;*/
   }
   .logo{
     width: 100%;
     /*margin: 20px;*/
     padding: 20px;
     display: flex;
     justify-content: center;
   }
 }
</style>
