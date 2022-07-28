<template>
  <div class="courseCard">
    <img :src="source" alt="guy with headphones" srcset="" class="courseImg" />
    <h3 class="courseTitle">
      {{ title }}
    </h3>
    <p class="enrollments">{{ enrollments }} Student</p>
    <div class="courseInfo">
      <div class="duration">
        <img src="../../assets/schedule-24px.svg" alt="timer" srcset="" />
        <p class="info">{{ duration }}</p>
      </div>
      <div class="lectures">
        <img src="../../assets/date_range-24px.svg" alt="calendar" srcset="" />
        <p class="info">{{ lectures }} lectures</p>
      </div>
    </div>
    <div class="authorInfo">
      <div class="avatar">
        <!-- <img src="" alt="" /> -->
        <p class="authorName">{{ author }}</p>
      </div>
      <div class="price">
        <p class="price">Rs. {{ price }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    source: String,
    title: String,
    enrollments: Number,
    duration: Number,
    lectures: Number,
    author: String,
    price: Number,
  },

  methods: {
    stringDuration() {},
  },
};
</script>

<style>
.courseCard {
  margin: 20px 0px;
  width: 300px;
  height: 600px;
  background: #ffffff 0% 0% no-repeat padding-box;
  border: 1px solid #e6e6e6;
  border-radius: 15px;
  opacity: 1;
  display: flex;
  flex-direction: column;
}

.courseCard img {
  width: 300px;
  border-radius: 15px 15px 0px 0px;
  opacity: 1;
  background: transparent;
  display: inline-block;
}

.courseCard p {
  display: inline-block;
}
.courseTitle {
  margin: 20px 15px;
  text-align: left;
  font: normal normal bold 25px Noto Sans;
  letter-spacing: 0px;
  color: #1f2532;
  opacity: 1;
}

.enrollments {
  margin: 10px 15px;
  text-align: left;
  letter-spacing: 0px;
  color: #1f2532;
  opacity: 1;
}

.courseInfo {
  display: flex;
  justify-content: space-between;
  margin: 0px 15px;
  padding: 20px 0px;
  border-bottom: 1px solid lightgray;
}

.courseInfo img {
  height: 24px;
  width: 24px;
}

.courseInfo .info {
  margin: 0;
}

.authorInfo {
  display: flex;
  justify-content: space-between;
  margin: 0px 15px;
  padding: 20px 0px;
}

.authorName {
  text-align: left;
  font: normal normal bold 20px Noto Sans;
  letter-spacing: 0px;
  color: #1f2532;
  opacity: 1;
}
</style>
