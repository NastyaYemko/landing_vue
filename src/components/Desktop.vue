<template>
  <section class="desktop">
    <div class="text">
      <div class="name-of-others">Listen on desktop or mobile</div>
      <div class="description-of-others">Lorem ipsum dolor sit amet, consectetur adipiscing elit. uisque ullamcorper porttitor blandit. Praesent lorem magna, fring</div>
    </div>
    <div class="imgs">
      <img class="phone" src="../assets/phone.png" alt="">
      <img src="../assets/desktop.png" alt="">
    </div>
  </section>
</template>

<script>
export default {
  name: "Desktop"
}
</script>

<style scoped>
.desktop{
  background: #09002B;
  height: 90vh;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}
.name-of-others{
  font-family: SF Pro Display;
  font-style: normal;
  font-weight: bold;
  font-size: 48px;
  line-height: 45px;
  text-align: center;
  color: #FFFFFF;

}
.description-of-others{
  font-family: SF Pro Display;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 19px;
  text-align: center;
  color: #FFFFFF;
  max-width: 460px;
  margin: 7px;
}
.imgs{
  display: flex;
  align-items: center;
justify-content: center;
  position: relative;
}
.phone{
  position: absolute;
  left: -150px;
  top: 84px;
}
</style>
