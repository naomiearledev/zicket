<template>
  <div class="home">
    <Jumbotron />
    <FeatureAbstract msg="Hello!" imgName="placeholder-screenshot.png"/>
  </div>
</template>

<script>
import TopBanner from '@/components/TopBanner.vue'
import Jumbotron from '@/components/Jumbotron.vue'
import FeatureAbstract from '@/components/FeatureAbstract.vue'

export default {
  name: 'HomeView',
  components: {
    TopBanner,
    Jumbotron,
    FeatureAbstract
  }
}
</script>