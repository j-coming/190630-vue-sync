<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <!-- <sync></sync> -->
    Home
    <dia-log :showDialog.sync="dialogFormVisible"/>

    <el-button type="text" @click="dialogFormVisible = true">打开嵌套表单的 Dialog</el-button>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Sync from "@/components/Sync.vue";
import diaLog from "@/components/dialog.vue";
export default {
  name: "home",
  components: {
    HelloWorld,
    Sync,
    diaLog
  },
  data() {
    return {
      dialogFormVisible: false
    };
  }
};
</script>
