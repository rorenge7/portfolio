<template>
  <div id="app">
    <Header />
    <section class="section">
      <b-container class="container">
        <router-view />
      </b-container>
    </section>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Header,
    Footer
  }
};
</script>

<style lang="scss">
@import "./styles/app.scss";

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

section {
  margin-bottom: 15em;
  @media (max-width: 767px) {
    margin-bottom: 22rem;
  }
}
</style>
