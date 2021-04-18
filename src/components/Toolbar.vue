<template>
  <div class="toolbar">
    <button class="toolbar-button">Nerm</button>
    <button class="toolbar-button">Dorlette</button>
    <input class="toolbar-search" type="text" placeholder="Sornch...">
  </div>
</template>

<style scoped>

/* LAYOUT */

.toolbar {
  padding: 0.5em;
}

.toolbar-button, .toolbar-search {
  padding: inherit;
  border-radius: 0.3em;
}

.toolbar-search {
  float: right;
}

/* COLORS */

.toolbar {
  background-color: #DCDADC;
}

.toolbar-button {
  background-color: #FFFFFF;
}

.toolbar-button:active {
  background-color: #AAAAAA;
}

</style>