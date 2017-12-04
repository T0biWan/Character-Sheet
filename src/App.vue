<template>
  <div id="app">
    <hero title="Heldendokument"></hero>
    <div <div class="container">
      <section>
        <div class="tile is-ancestor">
          <tile><box title="MU" value="10"></box></tile>
          <tile><box title="KL" value="10"></box></tile>
          <tile><box title="IN" value="10"></box></tile>
          <tile><box title="CH" value="10"></box></tile>
          <tile><box title="FF" value="10"></box></tile>
          <tile><box title="GE" value="10"></box></tile>
          <tile><box title="KO" value="10"></box></tile>
          <tile><box title="KK" value="10"></box></tile>
        </div>

      </section>
    </div>

  </div>
</template>

<script>
import hero from "./components/hero.vue"
import box from "./components/box.vue"
import tile from "./components/tile.vue"

export default {
  name: 'app',
  components: {
    'hero': hero,
    'box': box,
    'tile': tile,

  }
}
</script>

<style lang="scss"></style>
