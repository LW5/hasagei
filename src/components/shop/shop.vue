<template>


<el-container>
    
  <el-header>
    <el-menu  mode="horizontal" @select="handleSelect">
  <el-menu-item index="1">处理中心</el-menu-item>
   <el-menu-item index="4" disabled>2018-07-20</el-menu-item>
  <el-submenu index="2">
    <template slot="title">管理</template>
    <el-menu-item index="2-1">选项1</el-menu-item>
    <el-menu-item index="2-2">选项2</el-menu-item>
    <el-menu-item index="2-3">选项3</el-menu-item>
    <el-submenu index="2-4">
      <template slot="title">选项4</template>
      <el-menu-item index="2-4-1">选项1</el-menu-item>
      <el-menu-item index="2-4-2">选项2</el-menu-item>
      <el-menu-item index="2-4-3">选项3</el-menu-item>
    </el-submenu>
  </el-submenu>
  <el-menu-item index="3" >西瓜!欢迎回来</el-menu-item>
     <el-menu-item index="5">门店管理员</el-menu-item>
   
   
  

</el-menu>
<div class="line"></div>

  </el-header>


    <el-aside width="200px" >

        <el-row class="tac">
  <el-col >
   
    <el-menu
      default-active="2"
      class="el-menu-vertical-demo">
      <el-submenu index="1">
    <template slot="title">
      <i class="el-icon-location"></i>
      <span slot="title">商品管理</span>
    </template>
    <el-menu-item-group>
      <el-menu-item index="1-1">宠物</el-menu-item>
      <el-menu-item index="1-2">食品</el-menu-item>
      <el-menu-item index="1-3">用品</el-menu-item>
      <el-menu-item index="1-4">服务</el-menu-item>
    </el-menu-item-group>
   
  </el-submenu>
  
    <el-menu router mode="horizontal">
      <el-menu-item index="/Info/News">
        <i class="el-icon-menu"></i>
        <span slot="title">消息中心</span>
      </el-menu-item>
        <el-menu-item index="3">
        <i class="el-icon-menu"></i>
        <span slot="title">店员管理</span>
      </el-menu-item>
        <el-menu-item index="4">
        <i class="el-icon-menu"></i>
        <span slot="title">订单管理</span>
      </el-menu-item>
      </el-menu>
    </el-menu>
    
  </el-col>
  
</el-row>

 

</el-aside>
   
    
    <el-main>
        
    </el-main>
    <router-view></router-view> 
  


</el-container>



</template>

<script>
export default {
  //  methods: {
  //      data() {
  //   return {
  //     activeIndex: '1',
  //     activeIndex2: '1'
  //   };
  // },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
  
};
</script>

<style>
</style>


