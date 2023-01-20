<script>
import AppHeader from './components/AppHeader.vue';
import AppMainUp from './components/AppMainUp.vue';
export default {
  name: "App",
  data() {
    return {

    }
  },
  components: {
    AppHeader,
    AppMainUp
  }
};
</script>

<template>

  <app-header></app-header>
  <main>
    <app-main-up></app-main-up>
  </main>
  <footer></footer>

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

// UTILITY
.container {
  width: 70vw;
  margin: 0 auto;
}
</style>