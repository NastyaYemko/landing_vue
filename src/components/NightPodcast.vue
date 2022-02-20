<template>
  <section class="eath">
    <transition  appear name="bounce">
      <div class="night-podcast">
        <div class="name-of-night-podcast">Night Podcast</div>
        <div class="description-of-night-podcast">Listen to our Podcast at night after a tiring day</div>
        <img style="margin-top: 20px" src="../assets/podcast.png" alt="">
      </div>
    </transition>
  </section>
</template>

<script>
export default {
  name: "NightPodcast"
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
.eath{
  height: 100vh;
  background-image: url("../assets/background.png");
  background-size: cover;
}
.night-podcast{
  position: absolute;
  width: 565px;
  height: 262px;
  left: 67px;
  top: 330px;

}
.name-of-night-podcast{
  font-family: SF Pro Display;
  font-style: normal;
  font-weight: bold;
  font-size: 64px;
  line-height: 76px;
  color: #FFFFFF;
}

.description-of-night-podcast{
  font-family: SF Pro Display;
  font-style: normal;
  font-weight: 500;
  font-size: 36px;
  line-height: 43px;
  color: #FFFFFF;
}
</style>
