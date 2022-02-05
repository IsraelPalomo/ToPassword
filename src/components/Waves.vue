<template>
  <div class="Waves">
    <svg
      id="svg"
      viewBox="0 0 1440 400"
      xmlns="http://www.w3.org/2000/svg"
      class="transition duration-300 ease-in-out delay-150"
    >
      <path
        d="M 0,400 C 0,400 0,200 0,200 C 129.59999999999997,191.86666666666667 259.19999999999993,183.73333333333332 424,185 C 588.8000000000001,186.26666666666668 788.8,196.93333333333337 964,201 C 1139.2,205.06666666666663 1289.6,202.5333333333333 1440,200 C 1440,200 1440,400 1440,400 Z"
        stroke="none"
        stroke-width="0"
        fill="#7722ee88"
        class="transition-all duration-300 ease-in-out delay-150 path-1"
      ></path>

      <path
        d="M 0,400 C 0,400 0,300 0,300 C 188.66666666666663,300.1333333333333 377.33333333333326,300.2666666666667 533,297 C 688.6666666666667,293.7333333333333 811.3333333333335,287.06666666666666 957,287 C 1102.6666666666665,286.93333333333334 1271.3333333333333,293.4666666666667 1440,300 C 1440,300 1440,400 1440,400 Z"
        stroke="none"
        stroke-width="0"
        fill="#7722eeff"
        class="transition-all duration-300 ease-in-out delay-150 path-2"
      ></path>
    </svg>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";

@Component({})
export default class Waves extends Vue {}
</script>

<style lang="scss">
@import "../assets/scss/_waves.scss";
</style>
