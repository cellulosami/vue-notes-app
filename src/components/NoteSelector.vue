<template>
  <div 
    class="note-selector" 
    v-bind:class="{active: note.id === selectedNoteId}"
    v-on:click="selectNote(note)"
  >
    <p class="note-selector-title">{{ note.body }}</p>
    <p class="note-selector-timestamp">Tommshtulmp henrr...</p>
  </div>
</template>

<script>
export default {
  props: [
    "note",
    "selectedNoteId"
  ],
  methods: {
    selectNote: function (note) {
      console.log(`selected ${note.id}`);
      this.$emit("selectNote", note);
    }
  }
}
</script>

<style scoped>
/* .note-selector {
  padding: 1em;
}

.note-selector p {
  margin: 0;
} */

.note-selector {
  border-bottom: 1px solid #DCDADC;
}

.note-selector.active {
  background-color: #FCE18D;
}

.note-selector-title {
  background-color: inherit;
}

.note-selector-timestamp {
  color: #626262;
  background-color: inherit;
}

.note-selector-title {
  font-weight: bold;
}

.note-selector-timestamp {
  font-size: 0.7em;
}
</style>