<template>
  <div class="home">
    <Jumbotron />
  </div>
</template>

<script>
import TopBanner from '@/components/TopBanner.vue'
import Jumbotron from '@/components/Jumbotron.vue'

export default {
  name: 'HomeView',
  components: {
    TopBanner,
    Jumbotron
  }
}
</script>