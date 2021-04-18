<template>
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
</template>

<style scoped>

/* LAYOUT */

.note-selectors {
  flex: 0 0 13em;
}

.note-selector {
  padding: 1em;
}

.note-selector p {
  margin: 0;
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

/* TYPOGRAPHY */

.note-selector-title {
  font-weight: bold;
}

.note-selector-timestamp {
  font-size: 0.7em;
}

</style>