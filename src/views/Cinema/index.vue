<!-- 组件说明 -->
<template>
    <div id='main'>
        <Header title="喵喵影院"/>
        <div id="content">
            <div class="cinema_menu">
				<div class="city_switch">
					全城 <i class="iconfont icon-lower-triangle"></i>
				</div>
				<div class="brand_swtich">
					品牌 <i class="iconfont icon-lower-triangle"></i>
				</div>
				<div class="feature_switch">
					特色 <i class="iconfont icon-lower-triangle"></i>
				</div>
			</div>
            <CinemaList />
        </div>        
        <TabBar />
    </div>
</template>

<script>
    //import x from ''
    import Header from "@/components/Header";
    import TabBar from "@/components/TabBar";
    import CinemaList from "@/components/CinemaList";
    export default {
        name:'Cinema',
        components: {
            Header,
            TabBar,
            CinemaList
        },
        data () {
            return {

            };
        },
        computed: {

        },
        methods: {

        },
mounted() {

},
beforeCreate() {}, //生命周期 - 创建之前
beforeMount() {}, //生命周期 - 挂载之前
beforeUpdate() {}, //生命周期 - 更新之前
updated() {}, //生命周期 - 更新之后
beforeDestroy() {}, //生命周期 - 销毁之前
destroyed() {}, //生命周期 - 销毁完成
activated() {}, //如果页面有keep-alive缓存功能，这个函数会触发
    }
</script>

<style lang='scss' scoped>
//@import url()
#content .cinema_menu{ width: 100%; height: 45px; border-bottom:1px solid #e6e6e6; display: flex; justify-content:space-around; align-items:center; background:white;}
</style>