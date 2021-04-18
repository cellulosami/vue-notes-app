<template>
  <div class="note-selectors">
    <NoteSelector 
      v-for="note in notes" 
      v-bind:note="note" 
      v-bind:selectedNoteId="selectedNoteId" 
    />
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
      notes: [
        {id: 1, name: "Firmst", timestamp: Date.now() }, 
        {id: 2, name: "Sarcund", timestamp: Date.now() }, 
        {id: 3, name: "Throde", timestamp: Date.now() }
      ],
      selectedNoteId: 1
    }
  },
  methods: {
    selectNote: function (id) {
      this.selectedNoteId = id;
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