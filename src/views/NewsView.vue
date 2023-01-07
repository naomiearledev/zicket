<template>
  <Navigation />
  <div class="news">
    <h1>This is a news page</h1>
  </div>
</template>

<script>
import Navigation from '@/components/Navigation.vue'

export default {
  name: 'NewsView',
  components: {
    Navigation
  }
}
</script>