<template>
  <div v-if="loading">
    <Loader />
  </div>
  <div v-if="!loading">
    <Navbar />
    <ScrollTop />
    <ShowCase />
    <Box />
    <WatchGallery />
    <GalllerySection />
    <Gtr3Pro />
    <Gts3Pro />
    <TRexPro />
    <LearnDatabase />
    <Question />
    <Town />
    <ContactMaps />
    <Footer />
  </div>
</template>

<script>
import Loader from "./components/Loader.vue";
import Navbar from "./components/Navbar.vue";
import ShowCase from "./components/ShowCase.vue";
import Box from "./components/Box.vue";
import WatchGallery from "./components/WatchGallery.vue";
import Question from "./components/Question.vue";
import ScrollTop from "./components/ScrollTop.vue";
import ContactMaps from "./components/ContactMaps.vue";
import Gtr3Pro from "./components/Gtr3Pro.vue";
import Gts3Pro from "./components/Gts3Pro.vue";
import TRexPro from "./components/TRexPro.vue";
import Town from "./components/Town.vue";
import Footer from "./components/Footer.vue";
import GalllerySection from "./components/GalllerySection.vue";

export default {
  name: "App",
  components: {
    Loader,
    Navbar,
    ShowCase,
    Box,
    WatchGallery,
    Question,
    ScrollTop,
    ContactMaps,
    Gtr3Pro,
    Gts3Pro,
    TRexPro,
    Town,
    Footer,
    GalllerySection,
  },
  data: () => ({
    loading: true,
  }),
  mounted() {
    setTimeout(() => {
      document.querySelector(".loader").classList.add("fade-out");
      this.loading = false;
    }, 3000);
  },
};
</script>

<style>
body::before {
  display: block;
  content: "";
  height: 60px;
}

#map {
  width: 100%;
  height: 100%;
  border-radius: 10px;
}

@media (min-width: 576px) {
  .footer {
    padding: 0;
  }
}

@media (min-width: 290px) and (max-width: 500px) {
  .section {
    padding: 0rem;
  }
  .lead {
    font-size: 1rem;
  }
  p {
    font-size: 0.9rem;
  }
}
</style>
