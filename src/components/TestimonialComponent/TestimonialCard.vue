<template>
  <div class="testimonialCard">
    <p class="comment">
      {{ comment }}
    </p>
    <div class="testimonialBottom">
      <div class="info">
        <img
          src="../../assets/earners/christopher-campbell-rDEOVtE7vOs-unsplash.png"
          alt=""
          class="profile"
        />
        <p class="author">{{ author }}</p>
      </div>
      <img src="../../assets/right-quotation-sign.svg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    comment: String,
    author: String,
  },

  mounted() {
    console.log(this.comment);
  },
};
</script>

<style scoped>
.testimonialCard {
  box-shadow: 0px 20px 30px #1f25321a;
  border-radius: 15px;
  height: auto;
  width: 600px;
  padding: 30px 25px;
}

.comment {
  text-align: left;
  font: normal normal normal 20px Noto Sans;
  letter-spacing: 0px;
  color: #000000;
  text-transform: capitalize;
  opacity: 0.7;
  font-style: italic;
  display: inline-block;
}

img {
  height: 40px;
  width: 40px;
  border-radius: 50%;
  display: inline-block;
}

.testimonialBottom {
  display: flex;
  justify-content: space-between;
  margin-top: 20px;
}
</style>
