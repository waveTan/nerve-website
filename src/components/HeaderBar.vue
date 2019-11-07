<template>
  <el-row>
    <el-col class="logo">
      <img src="./../assets/logo.png">
    </el-col>
    <el-col class="menu">
      <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
        <el-menu-item index="1">场景</el-menu-item>
        <el-menu-item index="2">线路图</el-menu-item>
        <el-menu-item index="2">文档库</el-menu-item>
        <el-menu-item index="2">团队</el-menu-item>
        <el-menu-item index="2">白皮书</el-menu-item>
      </el-menu>
    </el-col>
  </el-row>
</template>

<script>
  export default {
    name: "header-bar",
    data() {
      return {
        activeIndex: '1',
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style scoped>

</style>
