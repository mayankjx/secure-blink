<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import HeroSection from "./components/HeroSection.vue";
import ContentSection from "./components/ContentSection.vue";
import CourseContainer from "./components/CourseComponents/CourseContainer.vue";
import EarnerContainer from "./components/EarnerComponents/EarnerContainer.vue";
import TestimonialContainer from "./components/TestimonialComponent/TestimonialContainer.vue";
import ContactContainer from "./components/ContactComponents/ContactContainer.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default {
  components: {
    HeaderComponent,
    HeroSection,
    ContentSection,
    CourseContainer,
    EarnerContainer,
    TestimonialContainer,
    ContactContainer,
    FooterComponent,
  },
};
</script>

<template>
  <header>
    <HeaderComponent></HeaderComponent>
  </header>
  <HeroSection></HeroSection>
  <div class="container c1">
    <div class="row">
      <ContentSection>
        <template #title>Courses</template>
        <template #subHeading>Our most popular courses</template>
        <template #container><CourseContainer></CourseContainer></template>
      </ContentSection>
    </div>
    <div class="row">
      <ContentSection>
        <template #title>Top Earners</template>
        <template #subHeading>Transformng your ideas into reality</template>
        <template #container><EarnerContainer></EarnerContainer></template>
      </ContentSection>
    </div>
    <div class="row">
      <ContentSection>
        <template #title>Refer</template>
        <template #subHeading>How It's Work</template>
        <template #container>
          <div class="banner">
            <img src="./assets/Group12142.png" alt="" />
          </div>
        </template>
      </ContentSection>
    </div>
    <div class="row">
      <ContentSection>
        <template #title>Testimonials</template>
        <template #subHeading
          >Check out What Our Students Think About Us</template
        >
        <template #container
          ><TestimonialContainer></TestimonialContainer
        ></template>
      </ContentSection>
    </div>
    <div class="row">
      <ContentSection>
        <template #title>Contact Us</template>
        <template #subHeading>Reach Out with any question you have</template>
        <template #container><ContactContainer></ContactContainer></template>
      </ContentSection>
    </div>
  </div>
  <FooterComponent></FooterComponent>
</template>

<style>
header {
  grid-column: 1/-1;
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: auto;
  z-index: 100;
}

.c1 {
  margin-top: 90px;
}

.row {
  margin: 10% auto;
}
</style>
