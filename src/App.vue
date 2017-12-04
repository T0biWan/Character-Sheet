<template>
  <div id="app">
    <hero title="Heldendokument"></hero>
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
