<template>
  <div class="jumbotron">
    <Navigation />
    <div class="jumbotron_primary-content">
      <h1>Make your event a success</h1>
      <p>Zicket handles all the hassle of selling tickets for every type of event</p>
      <router-link to="/get-zicket">
        <div class="jumbotron_primary-content_button">
          <span>Get Zicket &#10142;</span>
        </div>
      </router-link>
    </div>
    <div class="jumbotron_secondary-content">
      <hr>
      <p>Over 3,000,000 tickets sold at some of Asia's top events last year</p>
    </div>
  </div>
</template>

<script>
import Navigation from '@/components/Navigation.vue'

export default {
  name: 'Jumbotron',
  components: {
    Navigation
  },
  props: {

  }
}
</script>

<style lang="less">
.jumbotron {
  background: rgb(32,0,187);
  background: linear-gradient(126deg, rgba(32,0,187,1) 0%, rgba(44,13,111,1) 100%);
  height: 90vh;
  min-height: 600px;
  max-height: 950px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;

  &_primary-content {
    max-width: 600px;
    display: flex;
    flex-direction: column;
    align-items: center;

    h1 {
      color: #fff;
      font-family: Helvetica, sans-serif;
      font-size: 60px;
      font-weight: 400;
      line-height: 90%;
      -webkit-text-fill-color: transparent;
      -webkit-text-stroke-width: 1px;
      -webkit-text-stroke-color: #fff;
      margin-bottom: 1.5rem;
    }

    p {
      color: #fff;
      margin-bottom: 1.5rem;
      max-width: 400px;
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

  &_secondary-content {
    margin-bottom: 2rem;
    max-width: 450px;

    p {
      text-transform: uppercase;
      color: #fff;
      font-size: 12px;
      line-height: 150%;
      font-family: 'Montserrat', sans-serif;
      font-weight: 400;
    }
  }

  hr {
    border: none;
    height: 1px;
    background: rgb(148,148,148);
    background: linear-gradient(90deg, rgba(148,148,148,0) 0%, rgba(148,148,148,1) 50%, rgba(148,148,148,0) 100%);
    margin-bottom: 1rem; 
  }
}
</style>