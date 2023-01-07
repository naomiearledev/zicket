<template>
  <Navigation />
  <div class="home">
    <h1>This is a home page</h1>
  </div>
</template>

<script>
import TopBanner from '@/components/TopBanner.vue'
import Navigation from '@/components/Navigation.vue'

export default {
  name: 'HomeView',
  components: {
    TopBanner,
    Navigation
  }
}
</script>