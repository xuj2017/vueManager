<template>
  <el-breadcrumb separator="/">
  <el-breadcrumb-item :to="{ path: '/' }">首页</el-breadcrumb-item>
  <el-breadcrumb-item>数据管理</el-breadcrumb-item>
  <el-breadcrumb-item>成员列表</el-breadcrumb-item>
</el-breadcrumb>
</template>

<script>
export default {
  name: 'member',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>