<template>
  <div class="container">
    <div class="row">
      <div class="col" v-for="(earner, index) in earnerList" :key="index">
        <EarnerCard :source="earner.source" :money="earner.money"></EarnerCard>
      </div>
    </div>
  </div>
</template>

<script>
import EarnerCard from "./EarnerCard.vue";
import { earners } from "./earners.json";

export default {
  components: {
    EarnerCard,
  },
  data() {
    return {
      earnerList: earners,
    };
  },
  mounted() {
    console.log(this.earnerList.value);
  },
};
</script>

<style></style>
