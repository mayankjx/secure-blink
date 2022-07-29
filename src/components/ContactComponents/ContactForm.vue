<template>
  <div class="contactForm">
    <p>Fill up the form and our team will get back to you within 24 hours</p>
    <input
      type="text"
      name=""
      id=""
      placeholder="Name"
      v-model="formData.name"
    />
    <input
      type="email"
      name=""
      id=""
      placeholder="Email"
      v-model="formData.email"
    />
    <input
      type="text"
      name=""
      id=""
      placeholder="Phone"
      v-model="formData.phone"
    />
    <input
      type="text"
      name=""
      id=""
      placeholder="Subject"
      v-model="formData.subject"
    />
    <textarea
      name=""
      id=""
      cols="65"
      rows="10"
      placeholder="Message"
    ></textarea>
    <br />
    <button @click="formSubmit">Submit</button>
  </div>
</template>

<script>
import { reactive } from "vue";
import { computed } from "vue";
import useValidate from "@vuelidate/core";
import { required } from "@vuelidate/validators";

export default {
  setup() {
    const formData = reactive({
      name: "",
      email: "",
      phone: "",
      subject: "",
    });

    const rules = computed(() => {
      return {
        email: { required },
        name: { required },
        phone: { required },
        subject: { required },
      };
    });

    function containsAnyLetter(str) {
      return /[a-zA-Z]/.test(str);
    }

    const formSubmit = () => {
      if (formData.phone.length !== 10 && containsAnyLetter(formData.phone)) {
        alert(`failed`);
      }
      if (
        formData.name &&
        formData.email &&
        formData.phone &&
        formData.subject
      ) {
        alert(`Form submit`);
      } else {
        alert(`failed`);
      }
    };

    return {
      formData,
      formSubmit,
    };
  },
};
</script>

<style>
.contactForm {
  width: 50%;
  padding: 0px 40px;
  margin: 0px auto;
}
.contactForm p {
  text-align: center;
  font: normal normal bold 20px Noto Sans;
  letter-spacing: 0px;
  color: #201f23;
  opacity: 1;
  max-width: 80%;
}

.contactForm input {
  width: 40%;
  margin-right: 40px;
  margin-bottom: 20px;
  outline: none;
  background: none;
  padding: 10px 15px;
  border: none;
  border-bottom: 4px #01cb63 solid;
  font-style: italic;
  font-weight: 400;
}
</style>
