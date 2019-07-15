<template>
  <div id="app">
    <loadingScreen v-if="isLoading"></loadingScreen>
    <div>Hello World!</div>
  </div>
</template>

<script>
import loadingScreen from '@/components/loadingScreen.vue';

export default {
  data() {
    return {
      isLoading: true,
    };
  },
  beforeMount() {
    setTimeout(() => {
      this.isLoading = false;
    }, 3000);
  },
  components: {
    loadingScreen,
  },
};
</script>


<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
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
