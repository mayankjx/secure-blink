<template>
  <div class="contactContainer">
    <div class="contactInfo">
      <h3>Contact Information</h3>
      <div class="contactBlock">
        <img src="../../assets/Group 10748.svg" alt="" />
        <p>contact@coursepro.com</p>
      </div>
      <div class="contactBlock">
        <img src="../../assets/Group 10749.svg" alt="" />
        <p>1800-562-895, 1800-869-877</p>
      </div>
      <div class="contactBlock">
        <img src="../../assets/Group 10750.svg" alt="" />
        <p>102 Street, India</p>
      </div>
    </div>
    <ContactForm></ContactForm>
  </div>
</template>

<script>
import ContactForm from "./ContactForm.vue";

export default {
  components: {
    ContactForm,
  },
};
</script>

<style>
.contactContainer {
  height: 600px;
  width: 100vw;
  background: #f8f9fb 0% 0% no-repeat padding-box;
  opacity: 1;
  position: relative;
  left: -120px;
  display: flex;
  justify-content: space-evenly;
  padding: 50px 0px;
}

.contactInfo {
  width: 40%;
  position: relative;
  left: 150px;
}

.contactBlock {
  display: flex;
  align-items: center;
}

.contactBlock img {
  justify-self: flex-start;
  height: 72px;
}

.contactBlock p {
  justify-self: flex-end;
}
</style>
