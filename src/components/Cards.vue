<template>
  <section class="cards">
    <div class="plans">
      <transition appear
          name="custom-classes-transition"
          enter-active-class="animated tada"
          leave-active-class="animated bounceOutRight"
      >
    <img src="../assets/3.png" alt="">
      </transition>
      <transition appear
                  name="custom-classes-transition"
                  enter-active-class="animated tada"
                  leave-active-class="animated bounceOutRight"
      >
        <img src="../assets/2.png" alt="">
      </transition>
      <transition appear
                  name="custom-classes-transition"
                  enter-active-class="animated tada"
                  leave-active-class="animated bounceOutRight"
      >
        <img src="../assets/22.png" alt="">
      </transition>

    </div>
    <div><img src="../assets/button.png" alt=""></div>
  </section>
</template>

<script>
export default {
  name: "Cards"
}
</script>

<style scoped>
.cards{
  min-height: 680px;
  background: #09002B;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.plans{
  width: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}
img{
  margin: 10px;
}
</style>
