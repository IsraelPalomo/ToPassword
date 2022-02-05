<template>
  <div class="Login">
    <Waves class="waves" />
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import Waves from "@/components/Waves.vue";

@Component({
  components: {
    Waves,
  },
})
export default class Login extends Vue {}
</script>

<style lang="scss">
@import "../assets/scss/_login.scss";
</style>
