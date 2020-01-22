<template>
  <div>
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Main from "./components/Main.vue";
import Header from "./components/Header";
import Footer from "./components/Footer";
export default {
  components: {
    Main,
    Header,
    Footer
  }
};
</script>
<style lang="css">
/* general */

header,
main,
footer,
h1,
h2,
h3,
h4,
h5,
h6,
p {
  margin: 0;
  padding: 0;
}

body {
  max-width: 1200px;
  margin: auto;
  font-family: "Exo 2", sans-serif;
  padding: 7px;
}
* {
  box-sizing: border-box;
}
</style>
