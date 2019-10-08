<!-- 组件说明 -->
<template>
  <div class="Mine">
    <Header title="我的喵喵" />
    <div id="content">
      <Login />
    </div>

    <TabBar />
  </div>
</template>

<script>
//import x from ''
import Header from "@/components/Header";
import TabBar from "@/components/TabBar";
import Login from "@/components/Login";
export default {
  name: "Mine",
  components: {
    Header,
    TabBar,
    Login
  },
  data() {
    return {};
  },
  computed: {},
  methods: {},
  mounted() {},
  beforeCreate() {}, //生命周期 - 创建之前
  beforeMount() {}, //生命周期 - 挂载之前
  beforeUpdate() {}, //生命周期 - 更新之前
  updated() {}, //生命周期 - 更新之后
  beforeDestroy() {}, //生命周期 - 销毁之前
  destroyed() {}, //生命周期 - 销毁完成
  activated() {} //如果页面有keep-alive缓存功能，这个函数会触发
};
</script>

<style lang='scss' scoped>
//@import url()
</style>