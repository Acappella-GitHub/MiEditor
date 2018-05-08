<template>
  <div id="app-vue">
    <div id="toolbar">

    </div>
    <div id="sidebar">
      <hr>
    </div>
    <div id="editorbar">

    </div>
  </div>
</template>

<script>
  export default {
    name: 'app-vue'
  }
</script>

<style>
  #toolbar {
    position: absolute;
    width: 60px;
    height: 100%;
    background: #333;
  }

  #sidebar {
    position: absolute;
    top: 0;
    left: 60px;
    width: 290px;
    height: 100%;
    background: #222;
  }

  #editorbar {
    position: absolute;
    top: 0;
    left: 350px;
    right: 0;
    height: 100%;
    background: #111;
  }

  #sidebar hr {
    position: absolute;
    right: 0;
    margin: 0;
    width: 2px;
    height: 100%;
    background: #555;
    border: none;
  }
</style>
