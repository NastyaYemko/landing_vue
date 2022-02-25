<template>
  <transition name="slide-fade">
<div class="module_background" v-if="show" @click.stop="hideDialog">
  <div @click.stop class="module">
    <p class="button top">Home</p>
    <hr>
    <p class="button">Articles</p>
    <hr>
    <p class="button">Blog</p>
    <hr>
    <div class="social-networks">
      <div class="social-network"><img src="../../assets/instagram.png" alt=""></div>
      <div class="social-network"><img src="../../assets/facebook.png" alt=""></div>
      <div class="social-network"><img src="../../assets/net.png" alt=""></div>
    </div>
  </div>
</div>
    </transition>
</template>

<script>
export default {
  name: "Module",
  props: {
    show: {
      type: Boolean,
      required: true
    }
  },
  methods: {
    hideDialog(){
      this.$emit('update:show', false)
    }
  }
}
</script>

<style scoped>
.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
  /* .slide-fade-leave-active до версии 2.1.8 */ {
  transform: translateX(10px);
  opacity: 0;
}
.button{
  cursor: pointer;
  text-align: center;
  margin: 5px;
  font-size: 30px;
  line-height: 30px;
  transition: background 0.25s ease-in;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}
.button:hover,
.button:focus {
  transition: background 0.3s ease-out;
  background: #09002B;
  background: rgba(9, 0, 43, 0.5);
}

.button:focus {
  outline: 1px solid #fff;
  outline-offset: -4px;
}
.top{
  border-top-left-radius: 30px;
  border-top-right-radius: 30px;
}
.module_background{
  width: 100vw;
  height: 100vh;
  position: fixed;
  background: rgba(0, 0, 0, 0.5);
  z-index: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}
.module{
  width: 80%;
  height: 50%;
  border-radius: 30px;
  background: #904ab3;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  color: #FFFFFF;
}
.social-network{
  cursor: pointer;
  margin-left: 10px;
  margin-right: 10px;
  width: 30px;
  height: 30px;
  border-radius: 50%;
  background-color: #4303A4;
  display: flex;
  justify-content: center;
  align-items: center;
}
.social-networks{
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin: 10px;
}
</style>
