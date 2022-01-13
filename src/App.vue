<template>
  <div id="app">
      <Header />
      <Main />
      <Cta />
      <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Cta from "./components/Cta.vue";
import Footer from "./components/Footer.vue";


export default {
  name: "App",
  components: {
    Header,
    Main,
    Cta,
    Footer
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";

.container {
  width: 80%;
  margin: 0 auto;
}
</style>
