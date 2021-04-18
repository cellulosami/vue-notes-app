<template>
  <div id="app">
    <Toolbar />
    <NoteContainer 
      v-bind:notes="notes"
    />
  </div>
</template>

<script>
import Toolbar from "./components/Toolbar.vue"
import NoteContainer from "./components/NoteContainer.vue"

export default {
  name: 'app',
  components: {
    Toolbar,
    NoteContainer
  },
  data: function () {
    return {
      notes: [
        {id: 1, name: "Firmst", timestamp: Date.now() }, 
        {id: 2, name: "Sarcund", timestamp: Date.now() }, 
        {id: 3, name: "Throde", timestamp: Date.now() }
      ],
    }
  }
};
</script>

<style>

/* RESET */

* {
  margin: 0;
  padding: 0;
  border: 0;
  outline: none;
  box-sizing: border-box;
}

/* LAYOUT */

#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

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