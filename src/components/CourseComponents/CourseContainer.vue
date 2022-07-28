<template>
  <div class="container">
    <div class="row">
      <div class="col" v-for="(course, index) in courseList" :key="index">
        <CourseCard
          :source="course.source"
          :title="course.title"
          :enrollments="course.enrollments"
          :duration="course.duration"
          :lectures="course.lectures"
          :author="course.author"
          :price="course.price"
        ></CourseCard>
      </div>
    </div>
  </div>
</template>

<script>
import CourseCard from "./CourseCard.vue";
import { courseList as lists } from "../../../data";

export default {
  components: {
    CourseCard,
  },
  data() {
    return {
      courseList: lists,
    };
  },
  mounted() {
    console.log(this.courseList);
  },
};
</script>

<style></style>
