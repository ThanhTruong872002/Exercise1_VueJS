<template>
  <!-- Header  -->
  <comp-header />

  <!-- Hero  -->
  <comp-hero />

  <!-- Take Avantage  -->
  <comp-advantage />

  <!-- Our core Feature  -->
  <comp-feature />

  <!-- PortFolio  -->
  <comp-portfolio />

  <!-- What our clients say  -->
  <comp-client />

  <!-- <todo-list /> -->
  <!-- Footer  -->
  <comp-footer />
</template>

<script>
import CompHeader from "./components/Header/CompHeader.vue";
import CompFooter from "./components/Footer/CompFooter.vue";
import CompAdvantage from "./components/Advantage/CompAdvantage.vue";
import CompFeature from "./components/Feature/CompFeature.vue";
import CompPortfolio from "./components/Portfolio/CompPortfolio.vue";
import CompClient from "./components/ClientSay/CompClient.vue";
import TodoList from "./components/TodoList.vue";
import CompHero from "./components/Hero/CompHero.vue";

export default {
  components: {
    CompHeader,
    CompFooter,
    CompAdvantage,
    CompFeature,
    CompPortfolio,
    CompClient,
    TodoList,
    CompHero,
  },
};
</script>
<style></style>
