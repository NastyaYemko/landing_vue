<template>
<section>
  <div class="speaker">
  <div class="description">
    <transition  appear name="bounce">
      <div class="block">
        <div class="text">
        <div class="name-of-block">Listen from one of the best singers</div>
        <div class="description-of-block">Lorem ipsum dolor sit amet, consectetur adipiscing elit. uisque ullamcorper porttitor blandit. Praesent lorem magna, fring</div>
        <img style="margin-top: 20px" src="../assets/talkToUsButton.png" alt="">
        </div>
        </div>
    </transition>
  </div>
    <div class="img">
<!--  <img src="../assets/speaker.png" alt="">-->
    </div>
  </div>
</section>
</template>

<script>
export default {
  name: "Singers"
}
</script>

<style scoped>
.bounce-enter-active {
  animation: bounce-in .5s;
}
.bounce-leave-active {
  animation: bounce-in .5s reverse;
}
@keyframes bounce-in {
  0% {
    transform: scale(0.5);
  }
  50% {
    transform: scale(1.2);
  }
  100% {
    transform: scale(1);
  }
}
.img{
  width: 765px;
  height: 680px;
  background-image: url("../assets/speaker.png");
  background-size: cover;
}
.speaker{
  background: #11024B;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  /*display: grid;*/
  /*grid-template-columns: 1fr 1fr;*/
}
.description{
  display: flex;
  align-items: center;
  justify-content: center;
}
.block{
  max-width: 450px;
  margin: 97px;
}
.name-of-block{
  font-family: SF Pro Display;
  font-style: normal;
  font-weight: bold;
  font-size: 48px;
  line-height: 45px;
  color: #FFFFFF;
}

.description-of-block{
  font-family: SF Pro Display;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  color: #FFFFFF;
  margin-top: 10px;
}
</style>
