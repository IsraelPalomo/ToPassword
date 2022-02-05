<template>
  <div class="Login">
    <header>
      <UserIconAN />
    </header>
    <main>
      <InputLogin />
    </main>
    <Waves class="waves" />
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import Waves from "@/components/Waves.vue";
import UserIconAN from "@/components/UserIconLogin.vue";
import InputLogin from "@/components/InputLogin.vue";

@Component({
  components: {
    Waves,
    UserIconAN,
    InputLogin,
  },
})
export default class Login extends Vue {}
</script>

<style lang="scss">
@import "../assets/scss/_asset.scss";
@import "../assets/scss/_login.scss";
</style>
