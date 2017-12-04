<template>
  <div id="app">
    <hero title="Heldendokument"></hero>
    <!-- <eigenschaft title="MU">10</eigenschaft>
    <eigenschaft title="KL">10</eigenschaft>
    <eigenschaft title="IN">10</eigenschaft>
    <eigenschaft title="CH">10</eigenschaft>
    <eigenschaft title="FF">10</eigenschaft>
    <eigenschaft title="GE">10</eigenschaft>
    <eigenschaft title="KO">10</eigenschaft>
    <eigenschaft title="KK">10</eigenschaft> -->
    <personal-data></personal-data>
  </div>
</template>

<script>
import hero from "./components/hero.vue"
import eigenschaft from "./components/eigenschaft.vue"
import personal_data from "./components/personal_data.vue"

export default {
  name: 'app',
  components: {
    'hero': hero,
    'eigenschaft': eigenschaft,
    'personal-data': personal_data,
  }
}
</script>

<style lang="scss"></style>
