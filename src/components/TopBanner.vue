<template>
  <div class="top-banner">
    <p>Looking to buy tickets to an event?</p>
    <a href="~/tickets">Get them here</a>
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
  display: flex;
  justify-content: center;
  padding: 1rem 0;
  
  p {
    color: #B3A7E3;
    margin-right: 1rem;
  }

  a {
    color: #f93b84;
  }
}
</style>