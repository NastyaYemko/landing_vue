<template>
<section>
<div>
  <div class="name-of-column">Navigation</div>
  <div class="column">Home</div>
  <div class="column">Articles</div>
  <div class="column">Blog</div>
</div>
  <div>
  <div class="name-of-column">Our socials</div>
  <div class="column">Instagram</div>
  <div class="column">Spotify</div>
  <div class="column">Facebook</div>
</div>
  <div class="logo">
    <div class="ellipse">
      <span class="podcaster">Podcaster</span>
    </div>
  </div>
  <div>
  <div class="name-of-column">Usefull links</div>
  <div class="column">Privacy police</div>
  <div class="column">Terms & conditions</div>
  <div class="column">Exchange and return policy</div>
</div>
  <div>
  <div class="name-of-column">Information</div>
  <div class="column">About us</div>
  <div class="column">Contact us</div>
  <div class="column">Blogs</div>
  <div class="column">FAQ</div>
</div>
</section>
</template>

<script>
export default {
  name: "MyFooter"
}
</script>

<style scoped>
 section{
   background: #11024B;
   min-height: 60vh;
   display: flex;
   justify-content: space-around;
   align-items: center;
  flex-wrap: wrap;
 }
 .ellipse{
   width: 144px;
   height: 61px;
   background: #3531A9;
   border: 1px solid #000000;
   box-sizing: border-box;
   box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
   transform: rotate(-30deg);
   border-radius: 200%;
 }
 .podcaster{
   position: absolute;
   width: 154px;
   height: 58px;
   transform: rotate(30deg);
   font-family: Caveat;
   font-style: normal;
   font-weight: bold;
   font-size: 46px;
   line-height: 58px;
   color: #FFFFFF;
 }
 .name-of-column{
   font-family: SF Pro Display;
   font-style: normal;
   font-weight: bold;
   font-size: 18px;
   line-height: 21px;

   color: #3531A9;
 }
 .column{
   font-family: SF Pro Display;
   font-style: normal;
   font-weight: 500;
   font-size: 18px;
   line-height: 21px;
   margin-top: 21px;
   color: #FFFFFF;
 }
</style>
