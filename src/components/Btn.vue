<template>
  <div class="Btn">
    <p class="Btn__title">{{ text }}</p>
  </div>
</template>

<script lang="ts">
import { Vue, Component, Prop } from "vue-property-decorator";

@Component({})
export default class Btn extends Vue {
  @Prop()
  text!: string;
}
</script>

<style lang="scss">
@import "../assets/scss/_asset.scss";
@import "../assets/scss/_btn.scss";
</style>
