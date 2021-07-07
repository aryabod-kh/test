<style lang="scss" scoped>
.login-card {
  display: flex;
  height: 640px;
  width: 100%;
  padding: 12px;
  @include media(md) {
    width: 600px;
  }
  @include media(lg) {
    width: 960px;
  }
  @include media(xl) {
    width: 1150px;
  }
  .form-box {
    flex: 1;
    background: #fff;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 100px;
    @include media(md) {
      width: 600px;
    }
    @include media(lg) {
      width: 960px;
    }
    @include media(xl) {
      width: 1150px;
    }
    .logo {
      display: flex;
      align-items: center;
      font-size: 35px;
      color: #e60000;
      font-weight: 600;
      img {
        margin-right: 13px;
        width: 100px;
      }
    }
    .get-started {
      color: #333;
      div {
        font-size: 35px;
        font-weight: 600;
        margin-bottom: 5px;
      }
      span {
        font-weight: 500;
        font-size: 16px;
      }
    }
    .form {
      display: flex;
      flex-direction: column;
      input {
        height: 48px;
        border: 0.5px solid #afafb6;
        border-radius: 50px;
        padding: 0 16px;
        font-size: 16px;
        font-weight: 500;
        &::placeholder {
          color: #4f4f4f;
        }
      }
      .submit {
        margin-top: 30px;
        position: relative;
        border-radius: 50px;
        background: #bdbdbd;
        padding: 16px;
        height: 48px;
        box-shadow: none;
        border: none;
        font-size: 16px;
        font-weight: 500;
        color: #fff;
        cursor: pointer;
        img {
          position: absolute;
          right: 33px;
          width: 16px;
        }
      }
    }
  }
  .pic-box {
    flex: 0 0 45%;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}
</style>
<template>
  <div class="login-card">
    <div class="form-box">
      <div class="logo">
        <img src="/img/logo.png" alt />
        <div>MateMachine</div>
      </div>
      <div class="get-started">
        <div>Let’s Get Started</div>
        <span>You’ve been missed</span>
      </div>
      <div class="form">
        <input type="text" name="email" id="email" placeholder="Email" />
        <button class="submit">
          Next
          <img src="/img/arrow-right.png" alt />
        </button>
      </div>
    </div>
    <div class="pic-box">
      <img src="/img/login-wrapper.jpg" alt />
    </div>
  </div>
</template>
<script lang="ts">
import { Vue, Component, Prop, Watch, Emit, Ref } from "vue-property-decorator";

@Component({
  layout: "login"
})
export default class component_name extends Vue {}
</script>