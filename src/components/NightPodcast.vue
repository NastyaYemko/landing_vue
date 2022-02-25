<template>
  <section  class="eath">
    <div>
      <night-podcast-block class="night-podcast"/>
      <div class="night-podcast">
      </div>
    </div>
  </section>
</template>

<script>
import NightPodcastBlock from "./elements/NightPodcastBlock";
export default {
  name: "NightPodcast",
  components: {NightPodcastBlock}
}
</script>

<style scoped>
.eath{
  height: 100vh;
  background-image: url("../assets/background.png");
  background-size: cover;
}
.night-podcast{
  position: absolute;
  max-width: 565px;
  height: 262px;
  left: 67px;
  top: 330px;
}
</style>
