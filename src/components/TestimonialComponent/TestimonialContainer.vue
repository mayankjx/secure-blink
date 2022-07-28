<template>
  <div class="container">
    <div class="row">
      <div
        class="col"
        v-for="(testimonial, index) in testimonialList"
        :key="index"
      >
        <TestimonialCard
          :comment="testimonial.comment"
          :author="testimonial.author"
        ></TestimonialCard>
      </div>
    </div>
  </div>
</template>

<script>
import TestimonialCard from "./TestimonialCard.vue";
import { testimonials } from "./testimonials.json";

export default {
  components: {
    TestimonialCard,
  },
  data() {
    return {
      testimonialList: testimonials,
    };
  },
};
</script>

<style></style>
