<template>
  <div class="UserIconLogin">
    <user-icon size="5x" class="UserIconLogin__icon"></user-icon>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import { UserIcon } from "vue-feather-icons";

@Component({
  components: {
    UserIcon,
  },
})
export default class UserIconAN extends Vue {}
</script>

<style lang="scss">
@import "../assets/scss/_asset.scss";
@import "../assets/scss/_userIconLogin.scss";
</style>
