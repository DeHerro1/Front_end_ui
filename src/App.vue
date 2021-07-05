<template>
  <div id="app">
    <Nav />
    <WelcomePage />
    <Solutions />
    <SubSection />
    <MainContent />
    <Security />
    <Veryfy />
  </div>
</template>

<script>
import Nav from "./components/Nav.vue";
import WelcomePage from "./components/WelcomePage.vue";
import Solutions from "./components/Solutions.vue";
import SubSection from "./components/SubSection.vue";
import MainContent from "./components/MainContent.vue";
import Security from "./components/Security.vue";
import Veryfy from "./components/Veryfy.vue";

export default {
  name: "App",
  components: {
    Nav,
    WelcomePage,
    Veryfy,
    MainContent,
    Security,
    Solutions,
    SubSection,
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
  --default_color--: #1a1357;
  --btn_color--: #50b946;
}

html {
  width: 100%;
}
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif; */
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

@media (max-width: 400px) {
  #app {
    width: 420px;
  }
}
</style>
