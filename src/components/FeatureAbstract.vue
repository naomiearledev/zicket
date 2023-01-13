<template>
  <div class="feature-abstract">
    <h1>{{ msg }}</h1>
    <img :src="require(`../assets/${imgName}`)" alt="Something">
  </div>
</template>

<script>
export default {
  name: 'FeatureAbstract',
  props: {
    msg: String,
    imgName: String
  }
}
</script>

<style>

</style>