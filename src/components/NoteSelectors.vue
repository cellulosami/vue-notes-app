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
  props: ["notes", "selectedNoteId"],
  data: function() {
    return {
      
    }
  },
  methods: {
    selectNote: function (note) {
      this.$emit("selectNote", note);
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