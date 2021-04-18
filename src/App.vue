<template>
  <div id="app">
    <Map />
    <Toolbar />
    <NoteContainer 
      v-bind:notes="notes"
      v-bind:selectedNoteId="selectedNoteId"
      v-on:selectNote="selectNote"
    />
  </div>
</template>

<script>
import Toolbar from "./components/Toolbar.vue"
import NoteContainer from "./components/NoteContainer.vue"
import Map from "./components/Map.vue"

export default {
  name: 'app',
  components: {
    Toolbar,
    NoteContainer,
    Map,
  },
  data: function () {
    return {
      notes: [
        {id: 1, body: "Thars us am Firmst toast.", timestamp: Date.now() }, 
        {id: 2, body: "Thars us am Sarcund toast.", timestamp: Date.now() }, 
        {id: 3, body: "Thars us am Throde toast.", timestamp: Date.now() },
        {id: 4, body: "Thars us am Froth toast.", timestamp: Date.now() }
      ],
      selectedNoteId: 1
    }
  },
  methods: {
    selectNote: function (note) {
      this.selectedNoteId = note.id
    }
  }
};
</script>

<style>

/* RESET */

/* * {
  margin: 0;
  padding: 0;
  border: 0;
  outline: none;
  box-sizing: border-box;
} */

/* LAYOUT */

/* #app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
} */

/* COLORS */

* {
  color: #454545;
  background-color: #FAFAF8;
}

/* TYPOGRAPHY */

body {
  font-family: sans-serif;
}

</style>