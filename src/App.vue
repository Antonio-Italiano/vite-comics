<script>
import AppHeader from './components/AppHeader.vue';
import AppMainUp from './components/AppMainUp.vue';
import AppMainDown from './components/AppMainDown.vue';
import AppFooterUp from './components/AppFooterUp.vue';
export default {
  name: "App",
  data() {
    return {

    }
  },
  components: {
    AppHeader,
    AppMainUp,
    AppMainDown,
    AppFooterUp
  }
};
</script>

<template>

  <app-header></app-header>
  <main>
    <app-main-up></app-main-up>
    <app-main-down></app-main-down>
  </main>

  <footer>
    <app-footer-up></app-footer-up>
  </footer>

</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

// GENERICS
li {
  list-style-type: none;
}

a {
  text-decoration: none;
}

// UTILITY
.container {
  width: 70vw;
  margin: 0 auto;
}
</style>