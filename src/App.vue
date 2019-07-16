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
  mounted() {
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
</style>
