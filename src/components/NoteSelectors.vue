<template>
  <div class="note-selectors">
    <NoteSelector class="active" v-for="note in notes"/>
  </div>
</template>

<script>
import NoteSelector from "./NoteSelector.vue"

export default {
  components: {
    NoteSelector
  },
  data: function() {
    return {
      notes: ["Firmst", "Sarcund", "Throde"]
    }
  }
}
</script>

<style scoped>

/* LAYOUT */

.note-selectors {
  flex: 0 0 13em;
}



/* COLORS */

.note-selectors {
  border-right: 1px solid #DCDADC;
}



/* TYPOGRAPHY */



</style>