<template>
  <div class="note-selectors">
    <NoteSelector 
      v-for="note in notes" 
      v-bind:note="note" 
      v-bind:selectedNoteId="selectedNoteId" 
      v-on:selectNote="selectNote"
    />
  </div>
</template>

<script>
import NoteSelector from "./NoteSelector.vue"

export default {
  components: {
    NoteSelector
  },
  props: ["notes"],
  data: function() {
    return {
      selectedNoteId: 1
    }
  },
  methods: {
    selectNote: function (note) {
      this.selectedNoteId = note.id;
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

</style>