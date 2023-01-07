<template>
  <TopBanner />
  <router-view/>
</template>

<script>
  import TopBanner from '@/components/TopBanner.vue'
  import Navigation from '@/components/Navigation.vue'

  export default {
  name: 'App',
  components: {
    TopBanner,
    Navigation
  }
}
</script>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
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
