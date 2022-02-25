<template>
  <section class="desktop_and_mobile">
    <div class="description">
    <block  :name="name" :description="description" class="text">
    </block>
    </div>
    <div class="imgs">
      <div class="phone"></div>
      <div class="desktop"></div>
    </div>
  </section>
</template>

<script>
import Block from "./elements/Block";

export default {
  name: "Desktop",
  components: {Block},
  data(){
    return{
      name: 'Listen on desktop or mobile',
      description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. uisque ullamcorper porttitor blandit. Praesent lorem magna, fring'
    }
  },
}
</script>

<style scoped>
.desktop_and_mobile{
  background: #09002B;
  padding: 20px;
  height: 80vh;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.description{
  width: 50%;
  display: flex;
  justify-content: center;
}
.imgs{
  width: 50%;
  display: flex;
  align-items: center;
justify-content: center;
  position: relative;
}
.phone{
  width: 144px;
  height: 299px;
  background-image: url("../assets/phone.png");
  background-size: cover;
}
.desktop{
  width: 546px;
  height: 351px;
  background-image: url("../assets/desktop.png");
  background-size: cover;
}
.text{
  width: 638px;
}
@media screen and (min-width: 701px) {
  .phone{
    position: absolute;
    left: -20px;
    top: 120px;
  }
}
@media screen and (max-width: 700px) {
  .imgs{
    width: 100%;
  }
  .text{
    width: 90%;
  }
  .desktop{
    display: none;
  }
}
</style>
