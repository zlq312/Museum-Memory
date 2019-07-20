<template>
  <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
    <el-menu :default-openeds="['1', '3']">
      <el-submenu index="1">
        <template slot="title"><i class="el-icon-message"></i>展</template>
        <el-menu-item-group>
          <el-menu-item index="1-1">画</el-menu-item>
          <el-menu-item index="1-2">雕塑</el-menu-item>
          <el-menu-item index="1-3">当代艺术</el-menu-item>
          <el-menu-item index="1-4">其他</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-menu-item index="2-1"><i class="el-icon-menu"></i>博物馆</el-menu-item>
      <el-menu-item index="3-1"><i class="el-icon-setting"></i>人物</el-menu-item>
    </el-menu>
  </el-aside>
</template>

<script>

export default {
  name: 'Sidebar'
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.el-aside {
  color: #333;
}
</style>
