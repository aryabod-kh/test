<style lang="scss" scoped>
.login-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100vh;
  .login {
    width: 300px;
    height: 60px;
    background: #e60000;
    border-radius: 8px;
    box-shadow: none;
    border: none;
    color: #fff;
    font-size: 18px;
    cursor: pointer;
  }
}
</style>
<template>
  <div class="login-wrapper">
    <button class="login" @click="login">ورود</button>
  </div>
</template>

<script lang="ts">
import { Vue, Component, Prop, Watch, Emit, Ref } from "vue-property-decorator";

@Component
export default class component_name extends Vue {
  login() {
    this.$router.push("/login");
  }
}
</script>
