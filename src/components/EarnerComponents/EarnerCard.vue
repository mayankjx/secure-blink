<template>
  <div class="earnerCard">
    <img :src="source" alt="earner profile pic" class="profile" />
    <p class="money">Rs. {{ money }}</p>
  </div>
</template>

<script>
export default {
  props: {
    source: String,
    money: Number,
  },
  mounted() {
    console.log(this.source);
  },
};
</script>

<style>
.earnerCard {
  display: flex;
  flex-direction: column;
}

.profile {
  width: 300px;
  height: 300px;
  border-radius: 5px;
  opacity: 1;
}

.money {
  margin: 10px 0px;
  padding: 5px 10px;
  display: inline-block;
  border-left: 6px solid #01cb63;
}
</style>
