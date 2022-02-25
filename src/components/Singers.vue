<template>
<section>
  <div class="speaker">
  <div class="description">
    <block  :name="name" :description="description" class="block">
      <img src="../assets/talkToUsButton.png" alt="">
    </block>
  </div>
    <div class="img">
    </div>
  </div>
</section>
</template>

<script>
import Block from "./elements/Block";

export default {
  name: "Singers",
  components: {Block},
  data(){
    return{
      name: 'Listen from one of the best singers',
      description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. uisque ullamcorper porttitor blandit. Praesent lorem magna, fring'
    }
  },
}
</script>

<style scoped>
img{
  margin-top: 10px;
}
.img{
  width: 55%;
  background-image: url("../assets/speaker.png");
  background-size: 100%;
  background-repeat: no-repeat;
}
.speaker{
  background: #11024B;
  display: flex;
  justify-content: space-between;
}
.description{
  width: 45%;
  height: 60vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
.block{
  max-width: 450px;
  margin: 97px;
}
@media screen and (max-width: 800px) {
  .speaker{
    display: flex;
    flex-direction: column;
  }
  .description{
    height: 60vh;
    width: 100%;
  }
  .img{
    width: 100%;
    height: 70vh;
    background-size: 100%;
    background-repeat: no-repeat;
  }
}
</style>
