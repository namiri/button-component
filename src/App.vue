<template>
  <div id="app">
    <Btn bgColor="green" outline="false" icon=""  />
    <Btn bgColor="blue" outline="true" icon=""  />
    <Btn bgColor="white" outline="true" icon=""  />
  </div>
</template>

<script>
import Btn from "./components/Btn.vue";

export default {
  name: "App",
  components: {
    Btn,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
