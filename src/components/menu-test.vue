<template>
  <section>
    <el-menu>
      <div class="menu-test-single-file">
        <el-link @click="ctrlFileList">文件夹名称</el-link>
        <el-submenu class="menu-test-first-class-title" index="1">
          <template slot="title">
            <el-icon class="el-icon-plus"></el-icon>
          </template>
          <div>
            <el-menu-item index="1-1">新建项目</el-menu-item>
            <el-menu-item index="1-2">模板引用</el-menu-item>
            <el-menu-item index="1-3">文本导入</el-menu-item>
            <el-submenu index="1-4">
              <template slot="title">新建文件夹</template>
                <div class="menu-test-second-class-content">
                  <el-menu-item index="1-4-1">选项1</el-menu-item>
                  <el-menu-item index="1-4-1">选项2</el-menu-item>
                  <el-menu-item index="1-4-3">选项3</el-menu-item>
                  <el-menu-item index="1-4-4">选项4</el-menu-item>
                  <el-menu-item index="1-4-5">选项5</el-menu-item>
                  <el-menu-item index="1-4-6">选项6</el-menu-item>
                </div>
            </el-submenu>
          </div>
        </el-submenu>
      </div>
    </el-menu>
  </section>
</template>

<script>
export default {
  name: 'menu-test',

  data() {
    return {

    }
  },
  mounted() {}
}
</script>
<style>
.menu-test-single-file {
  width: 100px;
  display: flex;
  justify-content: space-between;
  align-content: center;
}
.menu-test-first-class-title {
  width: 30px;
  height: 30px;
}
.el-icon-arrow-down:before {
  content: ''!important;
}
.menu-test-single-file .el-submenu__title {
  padding: 7px 0px !important;
  line-height: 0px;
  height: 27px;
}
.el-menu-item {
  padding-left: 0px!important;
  min-width:138px !important;
}
.menu-test-single-file li ul {
  width: 100px;
  background-color: red;
}
.menu-test-first-class-title .menu-test-second-class-content {
  position: absolute;
  background-color: blue;
  top: -177px;
  left: 100px;

}
</style>