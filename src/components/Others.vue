<template>
  <section class="others">
    <div class="text">
        <div class="name-of-others">Hear what others say</div>
        <div class="description-of-others">Lorem ipsum dolor sit amet, consectetur adipiscing elit. uisque ullamcorper porttitor blandit. Praesent lorem magna, fring</div>
    </div>
      <img src="../assets/Image.png" alt="">
  </section>
</template>

<script>
export default {
  name: "Others"
}
</script>

<style scoped>
.others{
  background: #09002B;
  height: 90vh;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-direction: column;
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
</style>
