<!-- 组件说明 -->
<template>
    <header id ="header">
        <h1>{{title}}</h1>
    </header>
</template>

<script>
    //import x from ''
    export default {
        name:'Header',
        props:{
            title:{
                type: String,
                default:'喵喵电影'
            }
        },
        components: {

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
#header{
    width:100%;
    height: 50px;
    color: #fff;
    background: #e54847;
    border-bottom: 1px solid #e54847;
    position: relative;
}
#header h1{
    font-size: 18px;
    text-align: center;
    line-height: 50px;
    font-weight: normal;
}

</style>