<template>
  <div id="app">

    <!-- Header della pagina -->
    <Header/>

    <!-- Parte centrale dalla pagina -->
    <main>
      <ContentBlack/>
      <Main/>
    </main>
    
    <!-- Footer della pagina -->
    <footer>
      <Jumbo/>
      <Footer/>
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import ContentBlack from "./components/ContentBlack.vue";
import Main from "./components/Main.vue";
import Jumbo from "./components/Jumbo.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    ContentBlack,
    Main,
    Jumbo,
    Footer,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
