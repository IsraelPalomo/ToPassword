<template>
  <div class="InputLogin">
    <div class="InputLogin__container">
      <user-icon size="1.5x" class="InputLogin__icon"></user-icon>
      <input class="InputLogin__input" type="text" placeholder="User" />
    </div>
    <div class="InputLogin__container">
      <key-icon size="1.5x" class="InputLogin__icon"></key-icon>
      <input class="InputLogin__input" type="password" placeholder="Password" />
    </div>
    <a class="InputLogin__remember" href="#">Forgot your password?</a>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import { UserIcon, KeyIcon } from "vue-feather-icons";

@Component({
  components: {
    UserIcon,
    KeyIcon,
  },
})
export default class InputLogin extends Vue {}
</script>

<style lang="scss">
@import "../assets/scss/_asset.scss";
@import "../assets/scss/_inputlogin.scss";
</style>
