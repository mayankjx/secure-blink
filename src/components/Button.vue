<template>
  <button @click="handleClick" :class="type"><slot></slot></button>
</template>

<script>
export default {
  props: {
    type: String,
  },
  setup(props, { emit }) {
    function handleClick() {
      if (props.type === "login") {
        emit("handleLogin");
      }
      if (props.type === "register") {
        emit("handleRegister");
      }
    }

    return {
      handleClick,
    };
  },
};
</script>

<style>
button {
  display: inline-block;
  border: none;
  outline: none;
  font: normal normal bold 20px/27px Noto Sans;
  padding: 10px 10px 10px 10px;
  cursor: pointer;
  margin: 0 20px;
}

.login {
  text-align: left;
  letter-spacing: 0px;
  color: #1f2532;
  opacity: 1;
  background: none;
}

.register {
  background: #01cb63 0% 0% no-repeat padding-box;
  box-shadow: 0px 5px 15px #01cb6359;
  border-radius: 10px;
  opacity: 1;
  color: white;
  padding: 10px 20px 10px 20px;
  font-weight: 400;
  font-style: italic;
}
</style>
