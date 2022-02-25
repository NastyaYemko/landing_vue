<template>
  <div class="landing">
  <my-header></my-header>
  <night-podcast animation-type="zoom"/>
  <cards animation-type="zoom"/>
  <singers animation-type="zoom"/>
  <others animation-type="zoom"/>
  <desktop animation-type="zoom"/>
  <my-footer></my-footer>
  <end></end>
  </div>
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
@import url('http://fonts.cdnfonts.com/css/sf-pro-display');
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

</style>
