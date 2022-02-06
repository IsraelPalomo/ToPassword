<template>
  <div class="NavBar">
    <div class="NavBar__logo">
      <img src="../assets/img/padlock.png" alt="Logotipo NavBar" />
    </div>
    <div class="NavBar__actions">
      <div class="NavBar__actions__langs">
        <!--  <select class="NavBar__actions__langs" id="locale" v-model="$i18n.locale"> -->
        <div class="container__langs" v-if="view_lang">
          <div
            v-for="locale in locales"
            class="lang"
            :key="locale.key"
            :value="locale.key"
            :class="locale.key == $i18n.locale ? 'active' : ''"
            @click="($i18n.locale = locale.key), (view_lang = !view_lang)"
          >
            {{ locale.key }}
          </div>
        </div>
        <div class="lang lang-locale" @click="view_lang = !view_lang">
          {{ $i18n.locale }}
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";

@Component({})
export default class NavBar extends Vue {
  view_lang = false;
  locales = [
    { key: "es", label: "Español" },
    { key: "en", label: "English" },
    { key: "fr", label: "French" },
  ];

  // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
  created() {
    console.log(this.$i18n);
  }
}
</script>

<style lang="scss">
@import "../assets/scss/_asset.scss";
@import "../assets/scss/_navBar.scss";
</style>
