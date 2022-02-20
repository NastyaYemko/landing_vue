<template>
  <my-header></my-header>
  <night-podcast></night-podcast>
  <cards></cards>
  <singers></singers>
  <others></others>
  <desktop></desktop>
  <my-footer></my-footer>
  <end></end>
</template>

<script>
import MyHeader from "./components/MyHeader";
import NightPodcast from "./components/NightPodcast";
import Cards from "./components/Cards";
import Singers from "./components/Singers";
import Others from "./components/Others";
import Desktop from "./components/Desktop";
import MyFooter from "./components/MyFooter";
import End from "./components/End";
export default {
  components: {End, MyFooter, Desktop, Others, Singers, Cards, MyHeader, NightPodcast}
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Caveat&display=swap');
@font-face {
  font-display: auto;
  font-family: "SF Pro Display";
  src: local("SF Pro Display"), url("/fonts/sf-pro-display-cufonfonts/SFPRODISPLAYREGULAR.OTF");
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
;
}

</style>
