<template>
  <div class="list">
    <span class="name-of-column">{{ name }}</span>
    <span v-for="column in columns" :key="column" class="column">{{column}}</span>
  </div>
</template>

<script>
export default {
  name: "list",
  props: {
    name: {
      type: String,
      required: true
    },
    columns: {
      type: Array,
      required: true
    }
  }
}
</script>

<style scoped>
.list{
  font-family: SF Pro Display;
  font-style: normal;
  font-size: 18px;
  line-height: 21px;
  display: flex;
  flex-direction: column;
  height: 40%;
  justify-content: space-between;
}
.name-of-column{
  font-weight: bold;
  color: #3531A9;
}
.column{
  font-weight: 500;
  margin-top: 21px;
  color: #FFFFFF;
}
</style>
