<template>
  <div ref="target">
  <transition name="bounce">
    <div v-if="animate" class="animated-component">
      <div class="block">
        <p class="name-of-block">{{name}}</p>
        <p class="description-of-block">{{description}}</p>
        <slot/>
      </div>
    </div>
  </transition>
  </div>
</template>

<script>
import {onMounted, ref} from "vue";

export default {
  name: "Block",
  props: {
    animationType: {
      type: String,
      required: false,
      default: 'fade'
    },
    name: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
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
    transform: scale(0.5);
  }
  50% {
    transform: scale(1);
  }
  100% {
    transform: scale(1);
  }
}
.block{
  font-family: SF Pro Display;
  font-style: normal;
  color: #FFFFFF;
}
.name-of-block{
  font-weight: bold;
  font-size: 48px;
  line-height: 45px;
}
.description-of-block{
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  margin-top: 10px;
}
</style>
