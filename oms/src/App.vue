<template>
  <div id="app">
    <el-container>
      <el-aside width="300px">
        <Aside />
      </el-aside>
      <el-container>
        <el-header><Header /></el-header>
        <el-main>Main</el-main>
        <router-view/>
        <el-footer>Footer</el-footer>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import Aside from './components/Aside/Aside.vue';
import Header from './components/Header/Header.vue';
// import OfficeInfo from './components/OfficeInfo/OfficeInfo.vue';
export default {
  components: {
    Aside,
    Header,
    // OfficeInfo,
  }

}
</script>


<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
