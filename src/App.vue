<template>
  <div id="app">
      <el-container>
        <el-header>Header</el-header>
        <el-container class="app-container">
          <el-aside width="200px">
            <side-bar />
            <el-footer class="side-footer">side-footer</el-footer>
          </el-aside>
          <el-container>
            <el-main>Main</el-main>
            <el-footer>Footer</el-footer>
          </el-container>
        </el-container>
      </el-container>
  </div>
</template>

<script>
import SideBar from './sidebar/';

export default {
  components: {
    SideBar,
  },
  created(){

  },
  methods: {
  }
}
</script>

<style>
#app {
  font-family: Helvetica, sans-serif;
  text-align: center;
  height: 100%;
}

.el-container {
  width:100%;
}

.app-container {
  top: 60px;
  position: absolute;

  right: 0;
  bottom: 0;
  left: 0;
}

.el-header {
  position: absolute;
  background-color: cornsilk;
  height: 60px;
  left: 0;
  top:0;
  right: 0;
}

.el-aside {
  background-color: azure;
  height: 100%;
  min-height: 710px;
  width:300px;
}
.side-footer {
  position: absolute;
  bottom: 0;
  left: 0;
  height: 30px;
}
.el-main {
  background-color: cadetblue;
}
.el-footer {
  background-color: burlywood;
}
</style>
