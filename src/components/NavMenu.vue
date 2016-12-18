<template>
  <el-menu default-active="1" class="el-menu-demo" mode="horizontal" @select="handleSelect">
    <h3 class="menu-title">Wizwork</h3>
    <el-menu-item index="1">订单管理</el-menu-item>
    <!--<el-submenu index="2">
      <template slot="title">我的工作台</template>
      <el-menu-item index="2-1">选项1</el-menu-item>
      <el-menu-item index="2-2">选项2</el-menu-item>
      <el-menu-item index="2-3">选项3</el-menu-item>
    </el-submenu>-->
    <el-menu-item index="2">客户管理</el-menu-item>
  </el-menu>
</template>

<script>
  // console.log(this);
  import { bus } from '../utils/event';
  export default {
    methods: {
      handleSelect(key, keyPath) {
        this.$emit('selectMenu', key);
      },
    }
  }
</script>

<style>
  .el-menu-demo {
    padding-left: 10px;
  }
  .menu-title {
    display: inline-block;
    float: left;
    margin-right: 20px;
  }
</style>