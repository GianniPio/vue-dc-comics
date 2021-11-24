<template>
  <div id="app">
    <Header/>
    <ContentBlack/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import ContentBlack from "./components/ContentBlack.vue";

export default {
  name: "App",
  components: {
    Header,
    ContentBlack,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
