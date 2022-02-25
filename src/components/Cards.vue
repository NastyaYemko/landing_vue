<template>
  <section ref="target" class="cards">
    <div class="plans">
      <div class="window">
      <card>
        <div class="card first_card"></div>
      </card>
      </div>
      <div class="window">
      <card>
        <div class="card second_card"></div>
      </card>
      </div>
      <div class="window">
      <card>
        <div class="card third_card"></div>
      </card>
      </div>
    </div>
  </section>
</template>

<script>
import Card from "./elements/Card";
export default {
  name: "Cards",
  components: {Card},
}
</script>

<style scoped>
.card{
  width: 275px;
  height: 344px;
  /*margin: 20px;*/
}
.first_card{
  background-image: url("../assets/3.png");
}
.second_card{
  background-image: url("../assets/2.png");
}
.third_card{
  background-image: url("../assets/22.png");
}
.cards{
  background: #09002B;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.plans{
  min-height: 90vh;
  width: 100vw;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}
img{
  margin: 10px;
}
@media screen and (max-width: 590px) {
  .window{
    width: 100vw;
    height: 90vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
@media screen and (min-width: 591px) and (max-width: 901px) {
  .plans{
    height: 120vh;
  }
}

</style>
