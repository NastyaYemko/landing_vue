<template>
  <section class="navigate">
    <div class="pages">
      <div class="page">Home</div>
      <div class="page">Articles</div>
      <div class="page">Blog</div>
    </div>
    <div class="name">
      <div class="ellipse">
        <span class="podcaster">Podcaster</span>
      </div>
    </div>
    <div class="social-networks">
      <div class="social-network"><img src="../assets/instagram.png" alt=""></div>
      <div class="social-network"><img src="../assets/facebook.png" alt=""></div>
      <div class="social-network"><img src="../assets/net.png" alt=""></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MyHeader"
}
</script>

<style scoped>
.name{
  width: 20%;
  display: flex;
  justify-content: center;
  margin: 10px;
}
.navigate{
  background-color: #1C0030;
  display: flex;
  /*flex-direction: column;*/
  padding-top: 46px;
  flex-wrap: wrap;
}
.social-networks{
  width: 35%;
  display: flex;
  flex-direction: row;
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
.pages{
  width: 40%;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  flex-wrap: wrap;
  margin: 10px;
}
.page{
  font-family: SF Pro Display;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 21px;
  color: #FFFFFF;
}
</style>
