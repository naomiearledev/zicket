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

