<template>
  <div class="home">
    <Jumbotron />
    <FeatureAbstract imgName="feature_set-up-payment.png" stepNum="01" altText="3D rendered image of credit cards and mobile phone" title="Set up & Payments" text="Quickly build your dedicated events page in English & Chinese. Accept payments from all major providers through our safe and reliable checkout." leftImg="true"/>
    <FeatureAbstract imgName="feature_progress-promotion.png" stepNum="02" altText="3D rendered image of graph and social media icons" title="Progress & Promotion" text="View sales & audience data in real-time. Maximise even reach via Zicket's Social Media channels, eDM Database and partner network." leftImg="false"/>
    <FeatureAbstract imgName="feature_entry-rfid.png" stepNum="03" altText="3D rendered image of RFID entry band and scanner" title="Entry & RFID" text="Manage entry through our iOS and Android app. Take your event cashless with our best-in-class solution." leftImg="true"/>
    <FeatureAbstract imgName="feature_support-analysis.png" stepNum="04" altText="3D rendered image of laptop and messages" title="Support & Analysis" text="Omni-channel support for you and your customers. Post event in-sight, analysis and recommendations." leftImg="false"/>
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