<template>
  <div class="navigation">
    <nav>
      <router-link to="/">
        <img src="../assets/placeholder-screenshot.png">
      </router-link>
      <div class="navigation_links">
        <router-link to="/about">About</router-link>
        <router-link to="/features">Features</router-link>
        <router-link to="/clients">Clients</router-link>
        <router-link to="/news">News</router-link>
        <router-link to="/faqs">FAQs</router-link>
      </div>
      <router-link to="/get-zicket">
        <div class="navigation_button">
          <span>Get Zicket</span>
        </div>
      </router-link>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Navigation',
  props: {

  }
}
</script>

<style lang="less">
.navigation {
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
  }

  img {
    width: 150px;
  }

  a {
    font-size: 14px;
    font-weight: 400;
    text-decoration: none;
  }

  &_links a {
    margin: 0 1rem;

    &:hover {
      color: #F93B84;
    }
  }

  &_button {
    background-color: #F93B84;
    padding: 1rem 2.5rem;
    border-radius: 2rem;

    span {
      text-transform: uppercase;
      font-weight: 700;
      color: #fff;
    }
  }
}
</style>