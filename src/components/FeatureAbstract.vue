<template>
  <div v-if="leftImg === 'true'" class="feature-abstract left-image">
    <div class="feature-abstract_image">
      <img src="../assets/vector-background.svg" alt="none" class="svg" />
      <img :src="require(`../assets/${imgName}`)" :alt="altText" class="img" />
    </div>
    <div class="feature-abstract_content">
      <div class="feature-abstract_content_title">
        <span>{{ stepNum }}</span>
        <h3>{{ title }}</h3>
      </div>
      <p>{{ text }}</p>
      <router-link to="/features">Explore features <div class="border-arrow_wrapper"><span class="border-arrow_inner">&#10142;</span></div></router-link>
    </div>
  </div>
  <div v-else class="feature-abstract right-image">
    <div class="feature-abstract_content">
      <div class="feature-abstract_content_title">
        <span>{{ stepNum }}</span>
        <h3>{{ title }}</h3>
      </div>
      <p>{{ text }}</p>
      <router-link to="/features">Explore features <div class="border-arrow_wrapper"><span class="border-arrow_inner">&#10142;</span></div></router-link>
    </div>
    <div class="feature-abstract_image">
      <img src="../assets/vector-background.svg" alt="none" class="svg svg-right" />
      <img :src="require(`../assets/${imgName}`)" :alt="altText" class="img" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'FeatureAbstract',
  props: {
    imgName: String,
    stepNum: String,
    altText: String,
    title: String,
    text: String,
    leftImg: Boolean
  }
}
</script>

<style lang="less">
.feature-abstract {
  display: flex;
  max-width: 850px;
  margin: 0 auto;
  padding: 2rem 0;

  &_image {
    position: relative;
    width: 60%;
    text-align: center;

    .svg {
      position: absolute;
      z-index: -1;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%;);
      width: 80%;
    }

    .img {
      width: 60%;
    }

    .svg-right {
      transform: translate(-50%, -50%;) scaleX(-1);
    }
  }

  &_content {
    width: 50%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 0 2rem;

    &_title {
      margin-bottom: 1.5rem;
      position: relative;

      h3 {
        font-family: 'Open Sans', sans-serif;
        font-weight: 400;
        font-size: 1.5rem;
        color: #2A4789;
      }

      span {
        font-family: Arial, Helvetica, sans-serif;
        color: #F1F5FB;
        font-size: 3rem;
        font-weight: 500;
        position: absolute;
        z-index: -1;
        top: -1.2rem;
      }
    }

    p {
      font-family: 'Open Sans', sans-serif;
      line-height: 200%;
      font-size: 0.8rem;
      color: #2A4789;
      margin-bottom: 1.5rem;
    }

    a {
      color: #3B8EF9;
      text-transform: uppercase;
      font-size: 0.8rem;
    }

    .border-arrow_wrapper {
      display: inline-block;
      border: 1px solid #3B8EF9;
      padding: 0.2rem;
      border-radius: 50%;
      margin-left: 0.5rem;
    }

    .border-arrow_inner {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 2rem;
      width: 2rem;
      background-color: #F1F5FB;
      color: #3B8EF9;
      border-radius: 50%;
    }
  }
}
</style>