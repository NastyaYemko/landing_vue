<template>
  <div class="logo">
    <div class="ellipse">
      <span class="podcaster">Podcaster</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Podcaster"
}
</script>

<style scoped>
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
</style>
