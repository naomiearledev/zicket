<template>
  <div class="top-banner">
    <caption>
      <p>Looking to buy tickets to an event?</p>
      <a href="~/tickets">Get them here</a></caption>
  </div>
</template>

<script>
export default {
  name: 'TopBanner',
  props: {

  }
}
</script>

<style lang="less">
.top-banner {
  background-color: #2C0D6F;
  padding: 1.25rem 0;
  
  caption {
    color: #B3A7E3;
    display: flex;
    justify-content: center;
  }

  p {
    margin-right: 1rem;
  }

  a {
    color: #f93b84;
  }
}
</style>