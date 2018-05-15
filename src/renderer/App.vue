<template>
  <div id="app-vue">
    <div id="toolbar">
      <toolbar></toolbar>
    </div>

    <div id="sidebar">
      <filemanager></filemanager>
      <hr v-on:clink="stretch">
    </div>

    <div id="editorbar">
      <div id="codebar">

      </div>
      <div id="shellbar">
        <hr>
        <div id="shellbar-tab">
          <a id="console-tab">控制台</a><a id="console-tab">控制台</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import toolbar from './components/ToolBar/ToolBar'
  import filemanager from './components/SideBar/FileManager'

  export default {
    name: 'app-vue',
    components: {
      toolbar,
      filemanager
    }
  }
</script>

<style lang="scss">
  #toolbar {
    position: absolute;
    width: 60px;
    height: 100%;
    background: #333;
  }

  #sidebar {
    position: absolute;
    left: 60px;
    width: 290px;
    height: 100%;
    background: #222;
    overflow: hidden;
  }

  #editorbar {
    position: absolute;
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

  #codebar {
    position: absolute;
    width: 100%;
    height: 70%;
  }

  #shellbar {
    position: absolute;
    bottom: 0;
    width: 100%;
    height: 30%;
  }

  #shellbar hr {
    margin: 0;
    width: 100%;
    height: 2px;
    background: #555;
    border: none;
  }

  #shellbar-tab {
    width: 100%;
    height: 25px;
    background: #444;

    a {
      display: inline-block;
      padding: 5px;
      font-size: 14px;
      color: #BBB;
      background: #111;
    }
  }
</style>
