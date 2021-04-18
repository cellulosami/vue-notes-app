<template>
  <div class="note-container">
    <div class="note-selectors">
      <div class="note-selector active">
        <p class="note-selector-title">Firmst normt...</p>
        <p class="note-selector-timestamp">Tommshtulmp henrr...</p>
      </div>
      <div class="note-selector">
        <p class="note-selector-title">Sarcund normt...</p>
        <p class="note-selector-timestamp">Tommshtulmp henrr...</p>
      </div>
      <div class="note-selector">
        <p class="note-selector-title">Throde normt...</p>
        <p class="note-selector-timestamp">Tommshtulmp henrr...</p>
      </div>
    </div>
    <div class="note-editor">
      <p class="note-editor-info">Tommshtulmp henrr...</p>
      <textarea class="note-editor-input">
        Firmst normt... 

        Normt terxt henrr... 
      </textarea>
    </div>
  </div>
</template>

<style scoped>

/* LAYOUT */

.note-container {
  display: flex;
  flex: 1;
}

.note-selectors {
  flex: 0 0 13em;
}

.note-selector {
  padding: 1em;
}

.note-selector p {
  margin: 0;
}

.note-editor {
  display: flex;
  flex: 1;
  flex-direction: column;
}

.note-editor-info {
  padding: 0.5em;
  text-align: center;
}

.note-editor-input {
  display: flex;
  flex: 1;
  width: 100%;
  padding: 0 2em 0 2em;
}

/* COLORS */

.note-selectors {
  border-right: 1px solid #DCDADC;
}

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

.note-editor-info {
  color: #DCDADC;
}

/* TYPOGRAPHY */

.note-selector-title {
  font-weight: bold;
}

.note-selector-timestamp {
  font-size: 0.7em;
}

.note-editor, .note-editor-input {
  font-size: 0.9em;
}

</style>