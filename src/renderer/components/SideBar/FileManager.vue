<template>
  <div id="file-manager-vue">
    <h1>文件管理器</h1>
    <el-button id="open-file-button" type="primary" size="small">打开文件/文件夹</el-button>
    <div id="test">
      <el-button icon="el-icon-plus" size="mini" circle></el-button>
      <el-button icon="el-icon-refresh" size="mini" circle></el-button>
    </div>
    <div id="file-list">
      <ul>
        <li></li>
        <li></li>
        <li></li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {

  }
</script>

<style>
  #file-manager-vue {
    position: absolute;
    width: 100%;
    height: 100%;
    text-align: center;
  }

  #file-manager-vue h1 {
    margin: 0;
    height: 32px;
    font-size: 15px;
    font-weight: lighter;
    line-height: 36px;
    color: #DDD;
    background: #444;
  }

  #open-file-button {
    margin: 8px 0;
    height: 32px;
    border-radius: 0;
  }

  #test {
    width: 100%;
    height: 32px;
    background: #444;
  }

  #file-list {
    width: 100%;
    height: 100%;
    overflow: auto;
  }
</style>