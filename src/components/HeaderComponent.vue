<template>
  <div class="navigationBar">
    <img src="../assets/header-logo.svg" alt="logo" srcset="" />
    <div class="buttons">
      <Button @handleLogin="loginHandler" type="login">Login</Button>
      <Button @handleRegister="registerHandler" type="register"
        >Register</Button
      >
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";

export default {
  components: {
    Button,
  },

  methods: {
    loginHandler() {
      console.log(`Login method called`);
    },

    registerHandler() {
      console.log(`Register method called`);
    },
  },
};
</script>

<style>
.navigationBar {
  display: flex;
  height: auto;
  padding: 20px 140px;
  align-items: center;
  justify-content: space-between;
  background-color: white;
  border-bottom: 2px lightgray solid;
}

.navigationBar img {
  height: 50px;
  cursor: pointer;
}
</style>
