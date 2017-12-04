<template>
<div>
  <!-- <eintrag title="Familie"></eintrag>
    <eintrag title="Geburtsort"></eintrag>
    <eintrag title="Geburtsdatum"></eintrag>
    <eintrag title="Alter"></eintrag>
    <eintrag title="Geschlecht"></eintrag>
    <eintrag title="Spezies"></eintrag>
    <eintrag title="Größe"></eintrag>
    <eintrag title="Gewicht"></eintrag>
    <eintrag title="Haarfarbe"></eintrag>
    <eintrag title="Augenfarbe"></eintrag>
    <eintrag title="Kultur"></eintrag>
    <eintrag title="Profession"></eintrag>
    <eintrag title="Titel"></eintrag>
    <eintrag title="Sozialstatus"></eintrag>
    <eintrag title="Charakteristika"></eintrag>
    <eintrag title="Sonstige"></eintrag> -->
  <div v-for="entry in character.PersoenlicheDaten.Vita">
    <eintrag title="Name">{{entry}}</eintrag>
  </div>
</div>
</template>

<script>
import json from "../assets/DSA.json"
import eintrag from "./eintrag.vue"

export default {
  name: 'personal_data',
  components: {
    'eintrag': eintrag,
  },
  data() {
    return {
      character: json
    }
  }
}
</script>
