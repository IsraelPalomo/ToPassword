<template>
  <div class="Copy">
    <p class="Copy__title" v-t="'copy.title'"></p>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";

@Component({})
export default class Copy extends Vue {}
</script>

<style lang="scss">
@import "../assets/scss/_asset.scss";
@import "../assets/scss/_copy.scss";
</style>
