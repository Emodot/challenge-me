<template>
  <div class="container">
    <HeroSection />
    <HowItWorks />
    <VideoSection />
    <GetStarted />
    <MeetTheTeam />
    <WhyChooseUs />
    <DownloadApp />
    <Subscribe />
    <Footer />
  </div>
</template>

<script>
import DownloadApp from '../components/Homepage/DownloadApp.vue'
import GetStarted from '../components/Homepage/GetStarted.vue'
import HeroSection from '../components/Homepage/HeroSection.vue'
import HowItWorks from '../components/Homepage/HowItWorks.vue'
import MeetTheTeam from '../components/Homepage/MeetTheTeam.vue'
import Subscribe from '../components/Homepage/Subscribe.vue'
import VideoSection from '../components/Homepage/VideoSection.vue'
import WhyChooseUs from '../components/Homepage/WhyChooseUs.vue'
export default {
  components: {
    HeroSection,
    HowItWorks,
    VideoSection,
    GetStarted,
    MeetTheTeam,
    WhyChooseUs,
    DownloadApp,
    Subscribe
  }

}
</script>

<style scoped>

</style>
