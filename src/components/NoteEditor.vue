<template>
  <div class="note-editor">
    <p class="note-editor-info">Tommshtulmp henrr...</p>
    <textarea class="note-editor-input">
      Firmst normt... 

      Normt terxt henrr... 
    </textarea>
  </div>
</template>

<style scoped>

/* LAYOUT */

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

.note-editor-info {
  color: #DCDADC;
}

/* TYPOGRAPHY */

.note-editor, .note-editor-input {
  font-size: 0.9em;
}

</style>