<template>
  <div  ref="target">
  <transition
      name="bounce"
  >
    <div v-if="animate" class="animated-component">
      <slot/>
    </div>
  </transition>
  </div>
</template>
<script>
import {onMounted, ref} from "vue";

export default {
  name: "Card",
  props: {
    animationType: {
      type: String,
      required: false,
      default: 'fade'
    }
  },
  setup() {
    const target = ref();
    const animate = ref(false);
    const observer = new IntersectionObserver(
        ([entry]) => {
          animate.value = entry.isIntersecting;
        },
        {
          threshold: 0.5
        }
    );
    onMounted(() => {
      observer.observe(target.value);
    });
    return {
      animate,
      target
    };
  }
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
    transform: rotate(0.5turn);
  }
  50% {
    transform: rotate(0.7turn);
  }
  100% {
    transform: scale(1);
    transform: rotate(1turn);
  }
}
</style>
