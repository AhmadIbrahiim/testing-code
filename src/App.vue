<template>
  <div id="app" dir="rtl">
    <nav-Bar></nav-Bar>
    <Header />
  </div>
</template>
<script>
import navBar from "./components/navBar.vue";
import Header from "./components/header.vue";
export default {
  components: {
    navBar,
    Header,
  },
};
</script>

<style lang="scss">
@import url("http://fonts.cdnfonts.com/css/droid-arabic-naskh");
#app {
  font-family: "Droid Arabic Naskh", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>