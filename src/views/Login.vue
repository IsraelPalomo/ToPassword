<template>
  <div class="Login">
    <nav><NavBar /></nav>
    <header>
      <UserIconAN />
    </header>
    <main>
      <InputLogin />
      <Btn text="Login" />
    </main>
    <footer><Waves class="waves" /> <Copy /></footer>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import Waves from "@/components/Waves.vue";
import UserIconAN from "@/components/UserIconLogin.vue";
import InputLogin from "@/components/InputLogin.vue";
import NavBar from "@/components/NavBar.vue";
import Btn from "@/components/Btn.vue";
import Copy from "@/components/Copy.vue";

@Component({
  components: {
    Waves,
    UserIconAN,
    InputLogin,
    NavBar,
    Btn,
    Copy,
  },
})
export default class Login extends Vue {}
</script>

<style lang="scss">
@import "../assets/scss/_asset.scss";
@import "../assets/scss/_login.scss";
</style>
