<template>
<div class="menu-wrap">
<el-row class="tac">
            <el-col>
                <el-menu default-active="2" class="el-menu-vertical-demo  el-menu--dark" @open="handleOpen" @close="handleClose" style="    text-align: left;">
                    <el-submenu index="1">
                        <template slot="title">
                            <i class="el-icon-message"></i>
                            <span>数据管理</span>
                        </template>
                        <el-menu-item-group>
                            <el-menu-item index="1-1" @click="go('/member')">成员列表</el-menu-item>
                        </el-menu-item-group>
                        
                    </el-submenu>
                    <el-menu-item index="2">
                        <i class="el-icon-menu"></i>
                        <span slot="title">导航二</span>
                    </el-menu-item>
                    <el-menu-item index="3">
                        <i class="el-icon-setting"></i>
                        <span slot="title" :title="hello" :class="{hello}">{{hello}}</span>
                    </el-menu-item>
                </el-menu>
            </el-col>
        </el-row>
</div>
  
</template>
<script>
  export default {
    data(){
        return{
            hello:'world'
        }
    },
    methods: {
      handleOpen(key, keyPath) {
        // console.log(key, keyPath);
      },
      handleClose(key, keyPath) {
        // console.log(key, keyPath);
      },
      go(route) {
          this.$router.push({path:route})
      }
    }
  }
</script>

<style lang="scss" scoped>
    .menu-wrap{
        height: 100%;
            background-color: #324157;
    }
</style>


