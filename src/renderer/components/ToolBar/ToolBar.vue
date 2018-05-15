<template>
  <ul id="tool-bar-vue">
    <li><a id="icon-document" href="#icon-document"><i class="el-icon-document"></i></a></li>
    <li><a id="icon-setting" href="#icon-setting"><i class="el-icon-setting"></i></a></li>
  </ul>
</template>

<script>
  export default {

  }
</script>

<style lang="scss">
  #tool-bar-vue {
    margin: 0;
    padding: 0;
    list-style: none;

    li {
      height: 60px;

      a {
        display: block;
        font-size: 28px;
        text-align: center;
        line-height: 60px;
        color: #BBB;

        :hover {
          color: #FFF;
          cursor: pointer;
        }
      }
    }
  }

  #icon-document:target,#icon-setting:target {
    color: #FFF;
  }
</style>
