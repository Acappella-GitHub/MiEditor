<template>
  <ul id="tool-bar-vue">
    <li><i class="el-icon-document"></i></li>
    <li><i class="el-icon-setting"></i></li>
  </ul>
</template>

<script>
  export default {

  }
</script>

<style>
  #tool-bar-vue {
      margin: 0;
      padding: 0;
      width: 100%;
      list-style: none;
  }

  #tool-bar-vue li {
      height: 60px;
      text-align: center;
      line-height: 60px;
      font-size: 28px;
      color: #DDD;
  }

  #tool-bar-vue li:hover {
    color: #FFF;
  }
</style>
