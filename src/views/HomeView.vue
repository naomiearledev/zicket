<template>
  <div class="home">
    <Jumbotron />
    <div class="how-it-works">
      <div class="how-it-works_info">
        <div class="how-it-works_info_title">
          <h2>
            <span class="outline-text">how zicket</span>
            <span>works</span>
          </h2>
        </div>
        <div class="how-it-works_info_text">
          <p>Our Hong Kong and Singapore based experts will help you get your event set up and selling tickets quickly and easily.</p>
        </div>
      </div>
      <FeatureAbstract imgName="feature_set-up-payment.png" stepNum="01" altText="3D rendered image of credit cards and mobile phone" title="Set up & Payments" text="Quickly build your dedicated events page in English & Chinese. Accept payments from all major providers through our safe and reliable checkout." leftImg="true"/>
      <FeatureAbstract imgName="feature_progress-promotion.png" stepNum="02" altText="3D rendered image of graph and social media icons" title="Progress & Promotion" text="View sales & audience data in real-time. Maximise even reach via Zicket's Social Media channels, eDM Database and partner network." leftImg="false"/>
      <FeatureAbstract imgName="feature_entry-rfid.png" stepNum="03" altText="3D rendered image of RFID entry band and scanner" title="Entry & RFID" text="Manage entry through our iOS and Android app. Take your event cashless with our best-in-class solution." leftImg="true"/>
      <FeatureAbstract imgName="feature_support-analysis.png" stepNum="04" altText="3D rendered image of laptop and messages" title="Support & Analysis" text="Omni-channel support for you and your customers. Post event in-sight, analysis and recommendations." leftImg="false"/>
    </div>
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

<style lang="less">
  .how-it-works {
    max-width: 850px;
    margin: 0 auto;

    &_info {
      display: flex;
      padding: 5rem 0 2rem 0;

      &_title,
      &_text {
        width: 50%;
      }

      &_title {
        text-transform: uppercase;
        font-family: Helvetica, sans-serif;
        font-size: 1.5rem;
        display: flex;
        justify-content: center;

        span {
          display: block;
          font-weight: 500;
          line-height: 94%;
          color: #3B8EF9;

          &:nth-of-type(1) {
            -webkit-text-fill-color: #fff;
            -webkit-text-stroke-width: 1px;
            -webkit-text-stroke-color: #3B8EF9;
          }
        }
      }

      &_text {
        padding: 0 4rem;
        font-size: 0.8rem;
        line-height: 200%;
      }
    }
  }
</style>