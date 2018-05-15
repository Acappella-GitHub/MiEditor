<template>
  <div id="file-manager-vue">
    <h1>文件管理器</h1>
    <el-button id="open-file-button" type="primary" size="small">打开文件/文件夹</el-button>
    <div id="file-tool">
      <i id="add-file" class="el-icon-plus"></i>
      <i id="refresh-file" class="el-icon-refresh"></i>
    </div>
    <div id="file-list">
    </div>
  </div>
</template>

<script>
  export default {

  }
</script>

<style lang="scss">
  #file-manager-vue {
    position: absolute;
    width: 100%;
    height: 100%;
    text-align: center;

    h1 {
      margin: 0;
      height: 32px;
      font-size: 15px;
      font-weight: lighter;
      line-height: 36px;
      color: #CCC;
      background: #444;
    }
  }

  #open-file-button {
    margin: 8px 0;
    height: 32px;
    border-radius: 0;
  }

  #file-tool {
    width: 100%;
    height: 32px;
    font-size: 0;
    text-align: right;
    line-height: 46px;
    background: #444;
  }

  #add-file,#refresh-file {
    margin: 0 12px 0 0;
    font-size: 20px;
    color: #CCC;
  }

  #add-file:hover,#refresh-file:hover {
    color: #FFF;
    cursor: pointer;
  }

  #file-list {
    width: 100%;
    height: 100%;
    overflow: auto;
  }
</style>