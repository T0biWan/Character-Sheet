<template>
  <div id="app">
    <hero title="Heldendokument"></hero>
    <div <div class="container">
      <section>
        <div class="tile is-ancestor">
          <tile><box title="MU" v-bind:value="char.Eigenschaften.MU"></box></tile>
          <tile><box title="KL" v-bind:value="char.Eigenschaften.KL"></box></tile>
          <tile><box title="IN" v-bind:value="char.Eigenschaften.IN"></box></tile>
          <tile><box title="CH" v-bind:value="char.Eigenschaften.CH"></box></tile>
          <tile><box title="FF" v-bind:value="char.Eigenschaften.FF"></box></tile>
          <tile><box title="GE" v-bind:value="char.Eigenschaften.GE"></box></tile>
          <tile><box title="KO" v-bind:value="char.Eigenschaften.KO"></box></tile>
          <tile><box title="KK" v-bind:value="char.Eigenschaften.KK"></box></tile>
        </div>

          <div class="tile is-ancestor">
            <div class="tile is-vertical box">
              <div class="tile is-child"><p>Name: {{char.PersoenlicheDaten.Vita.Name}}</p></div>
              <div class="tile is-child"><p>Familie: {{char.PersoenlicheDaten.Vita.Familie}}</p></div>
              <div class="tile is-child"><p>Geburtsort: {{char.PersoenlicheDaten.Vita.Geburtsort}}</p></div>
              <div class="tile is-child"><p>Geburtsdatum: {{char.PersoenlicheDaten.Vita.Geburtsdatum}}</p></div>
              <div class="tile is-child"><p>Alter: {{char.PersoenlicheDaten.Vita.Alter}}</p></div>
              <div class="tile is-child"><p>Geschlecht: {{char.PersoenlicheDaten.Vita.Geschlecht}}</p></div>
              <div class="tile is-child"><p>Spezies: {{char.PersoenlicheDaten.Vita.Spezies}}</p></div>
              <div class="tile is-child"><p>Größe: {{char.PersoenlicheDaten.Vita.Größe}}</p></div>
              <div class="tile is-child"><p>Gewicht: {{char.PersoenlicheDaten.Vita.Gewicht}}</p></div>
            </div>
            <div class="tile is-vertical box">
              <div class="tile is-child"><p>Haarfarbe: {{char.PersoenlicheDaten.Vita.Haarfarbe}}</p></div>
              <div class="tile is-child"><p>Augenfarbe: {{char.PersoenlicheDaten.Vita.Augenfarbe}}</p></div>
              <div class="tile is-child"><p>Kultur: {{char.PersoenlicheDaten.Vita.Kultur}}</p></div>
              <div class="tile is-child"><p>Profession: {{char.PersoenlicheDaten.Vita.Profession}}</p></div>
              <div class="tile is-child"><p>Titel: {{char.PersoenlicheDaten.Vita.Titel}}</p></div>
              <div class="tile is-child"><p>Sozialstatus: {{char.PersoenlicheDaten.Vita.Sozialstatus}}</p></div>
              <div class="tile is-child"><p>Charakteristika: {{char.PersoenlicheDaten.Vita.Charakteristika}}</p></div>
              <div class="tile is-child"><p>Sonstige: {{char.PersoenlicheDaten.Vita.Sonstige}}</p></div>
            </div>
            <div class="tile is-vertical">
              <div class="tile is-child"><box title="Erfahrungsgrad" v-bind:value="char.PersoenlicheDaten.Erfahrungsgrad"></box></div>
              <div class="tile is-child"><box title="AP gesamt" v-bind:value="char.PersoenlicheDaten.AP_gesamt"></box></div>
              <div class="tile is-child"><box title="AP gesammelt" v-bind:value="char.PersoenlicheDaten.AP_gesammelt"></box></div>
              <div class="tile is-child"><box title="Ap ausgegeben" v-bind:value="char.PersoenlicheDaten.Ap_ausgegeben"></box></div>
            </div>
          </div>
      </section>
    </div>

  </div>
</template>

<script>
import json from "./assets/DSA.json"

import hero from "./components/hero.vue"
import box from "./components/box.vue"
import tile from "./components/tile.vue"

export default {
  name: 'app',
  components: {
    'hero': hero,
    'box': box,
    'tile': tile,
  },
  data() {
    return {
      char: json
    };
  },
}
</script>

<style lang="scss"></style>
