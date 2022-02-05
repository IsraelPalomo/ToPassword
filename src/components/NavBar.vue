<template>
  <div class="NavBar">
    <div class="NavBar__logo">
      <img src="../assets/img/padlock.png" alt="Logotipo NavBar" />
    </div>
    <div class="NavBar__actions">
      <div class="NavBar__actions__langs">
        <span class="lang">ES</span>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";

@Component({})
export default class NavBar extends Vue {}
</script>

<style lang="scss">
@import "../assets/scss/_asset.scss";
@import "../assets/scss/_navBar.scss";
</style>
