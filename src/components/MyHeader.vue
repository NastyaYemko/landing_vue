<template>
  <module v-model:show="dialogVisible"/>
  <section class="navigate">
    <div class="pages">
      <p class="page">Home</p>
      <p class="page">Articles</p>
      <p class="page">Blog</p>
    </div>
    <div class="hamburger" @click="showDialog"></div>
    <div class="name">
     <podcaster/>
    </div>
    <div class="social-networks">
      <div class="social-network"><img src="../assets/instagram.png" alt=""></div>
      <div class="social-network"><img src="../assets/facebook.png" alt=""></div>
      <div class="social-network"><img src="../assets/net.png" alt=""></div>
    </div>
  </section>
</template>

<script>
import Podcaster from "./elements/Podcaster";
import Module from "./elements/Module";
export default {
  name: "MyHeader",
  components: {Module, Podcaster},
  data(){
    return{
      dialogVisible: false
    }
  },
  methods: {
    showDialog() {
      this.dialogVisible = !this.dialogVisible
    }
  }
}
</script>

<style scoped>

.navigate{
  background-color: #1C0030;
  display: flex;
  padding-top: 46px;
}
.name{
  width: 20%;
  display: flex;
  justify-content: center;
  margin: 10px;
}
.social-network{
  margin-left: 15px;
  width: 30px;
  height: 30px;
  border-radius: 50%;
  background-color: #4303A4;
  display: flex;
  justify-content: center;
  align-items: center;
}
.page{
  font-family: SF Pro Display;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 21px;
  color: #FFFFFF;
}
@media screen and (max-width: 700px) {
  .navigate{
    display: flex;
    justify-content: space-around;
  }
  .pages, .social-networks{
    display: none;
  }
  .hamburger{
    background-image: url("../assets/hamburger.png");
    width: 48px;
    height: 48px;
    cursor: pointer;
  }
}
@media screen and (min-width: 701px) {
  .hamburger{
    display: none;
  }
  .social-networks{
    width: 25%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin: 10px;
  }
  .pages{
    width: 40%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    flex-wrap: wrap;
    margin: 10px;
  }
}
</style>
