<!-- 组件说明 -->
<template>
  <div id="main">
    <Header title="喵喵电影" />
    <div id="content">
      <div class="movie_menu">
        <router-link tag="div" to="/movie/city" class="city_name">
          <span>郑州</span>
          <i class="iconfont icon-lower-triangle"></i>
        </router-link>
        <div class="hot_swtich">
          <router-link tag="div" to="/movie/nowPlaying" class="hot_item active">正在热映</router-link>
          <router-link tag="div" to="/movie/comingSoon" class="hot_item">即将上映</router-link>
        </div>
        <router-link tag="div" to="/movie/search" class="search_entry">
          <i class="iconfont icon-sousuo"></i>
        </router-link>
      </div>
      <keep-alive>
          <router-view />
      </keep-alive>
    </div>
    <TabBar />
  </div>
</template>

<script>
import Header from "@/components/Header";
import TabBar from "@/components/TabBar";
//import x from ''
export default {
  name: "Movie",
  components: {
    Header,
    TabBar
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
#content .movie_menu{width:100%;height: 45px;border-bottom:1px solid #e6e6e6; display: flex; justify-content: flex-start;}
.movie_menu .city_name{margin-left: 20px;height: 100%;line-height:45px;}
.movie_menu .city_name.router-link-active{color: #ef4238;border-bottom: 2px #ef4238 solid;}
.movie_menu .hot_swtich{display: flex;height: 100%;line-height: 45px}
.movie_menu .hot_item{font-size:15px;color:#666;width:80px;text-align: center;margin: 0 12px;font-weight: 700}
.movie_menu .hot_item.router-link-active{color:#ef4238;border-bottom: 2px #ef4238 solid;}
.movie_menu .search_entry{margin-right: 20px;height: 100%;line-height: 45px;}
.movie_menu .search_entry.router-link-active{color:#ef4238;border-bottom: 2px #ef4238 solid;}
.movie_menu .search_entry i{font-size:24px;color:red;}
</style>