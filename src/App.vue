<template>
  <!-- Header  -->
  <comp-header />

  <!-- Take Avantage  -->
  <comp-advantage />

  <!-- Our core Feature  -->
  <comp-feature />

  <!-- PortFolio  -->
  <comp-portfolio />

  <!-- What our clients say  -->
  <comp-client />

  <!-- Footer  -->
  <comp-footer />
</template>

<script>
import CompHeader from "./components/CompHeader.vue";
import CompFooter from "./components/CompFooter.vue";
import CompAdvantage from "./components/CompAdvantage.vue";
import CompFeature from "./components/CompFeature.vue";
import CompPortfolio from "./components/CompPortfolio.vue";
import CompClient from "./components/CompClient.vue";
export default {
  components: {
    CompHeader,
    CompFooter,
    CompAdvantage,
    CompFeature,
    CompPortfolio,
    CompClient,
  },
};
</script>
<style scoped></style>
