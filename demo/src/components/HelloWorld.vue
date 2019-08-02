<template>

  <el-container style="position: absolute;width:100%; height:100%;">
    <el-header>
      <el-button style="margin-top: 10px;margin-right: 20px;float: right;" type="danger" plain >按钮</el-button>
    </el-header>
    <el-container style="width:100%; height:100%;">
    <el-aside width=200px>
        <el-menu
          default-active="2"
          class="el-menu-vertical-demo"
          @open="handleOpen"
          @close="handleClose">

          <el-submenu index="1">
            <template slot="title">
              <i class="el-icon-user-solid"></i>
              <span>爬取规则</span>
            </template>
            <el-menu-item index="1-1">
              <i class="el-icon-user"></i>
              <span slot="title">新闻类</span>
            </el-menu-item>
            <el-menu-item index="1-2">
              <i class="el-icon-user"></i>
              <span slot="title">图片类</span>
            </el-menu-item>
          </el-submenu>
          <el-submenu index="2">
            <template slot="title">
              <i class="el-icon-date"></i>
              <span>定时调度</span>
            </template>
            <el-menu-item index="2-1">
              <i class="el-icon-date"></i>
              <span slot="title">任务列表</span>
            </el-menu-item>
          </el-submenu>
        </el-menu>
    </el-aside>
    <el-main>
      cccmain
    </el-main>
    </el-container>
  </el-container>

</template>
<script>
  export default {
    data() {
      return {
      }
    }
  };
</script>
<style scoped>
  .el-header {
    background-color: #24292e;
    color: #24292e;

  }
  .el-main {
    background-color: #E9EEF3;
    color: #24292e;
    text-align: center;
    line-height: 160px;
  }
  .el-aside {
    color: #24292e;

  }
</style>
