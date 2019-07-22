<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Dialog ref="Dia" />
    <el-button @click="handleOpen">点击弹出框</el-button>
  </div>
</template>

<script>
// @ is an alias to /src
import Dialog from '../components/Dialog/Dialog.vue'
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld,
    Dialog,
  },
  methods: {
    handleOpen() {
      this.$refs.Dia.open();
    }
  }
}
</script>
