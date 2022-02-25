<template>
  <section class="others">
    <block  :name="name" :description="description" class="text">
    </block>
    <div class="img"></div>
  </section>
</template>

<script>
import Block from "./elements/Block";

export default {
  name: "Others",
  components: {Block},
  data(){
    return{
      name: 'Hear what others say',
      description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. uisque ullamcorper porttitor blandit. Praesent lorem magna, fring'
    }
  },
}
</script>

<style scoped>
.img{
  width: 617px;
  height: 342px;
  background-image: url("../assets/Image.png");
  background-size: cover;
}
.others{
  background: #09002B;
  height: 90vh;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-direction: column;
}
.text{
  max-width: 477px;
}
@media screen and (max-width: 700px) {
  .img{
    width: 100%;
    background-size: 100%;
    background-repeat: no-repeat;
  }
  .text{
    width: 90%;
  }
}
</style>
