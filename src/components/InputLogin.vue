<template>
  <div class="InputLogin">
    <div class="InputLogin__container">
      <user-icon size="1.5x" class="InputLogin__icon"></user-icon>
      <input class="InputLogin__input" type="text" placeholder="Name" />
    </div>
    <div class="InputLogin__container">
      <key-icon size="1.5x" class="InputLogin__icon"></key-icon>
      <input class="InputLogin__input" type="password" placeholder="Password" />
    </div>
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
.InputLogin {
  width: 100%;
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
  justify-content: center;
  justify-items: center;
  margin-top: 5rem;

  .InputLogin__container {
    position: relative;
    display: flex;
    align-items: center;
    .InputLogin__input {
      height: 2rem;
      width: 100%;
      min-width: 17rem;
      border-radius: 5px;
      border: none;
      outline: none;
      text-align: center;
    }
    .InputLogin__icon {
      position: absolute;
      padding: 0.5rem;
      background-color: #7400b4;
      border-radius: 5px;
      color: #fff;
    }
  }
}
</style>
