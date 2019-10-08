<!-- 组件说明 -->
<template>
    <div class='我的喵喵'>
        <div class="login_body">
				<div>
					<input class="login_text" type="text" placeHolder="账户名/手机号/Email" >
				</div>
				<div>
					<input class="login_text" type="password" placeHolder="请输入您的密码" >
				</div>
				<div class="login_btn">
					<input type="submit" value="登录">
				</div>
				<div class="login_link">
					<a href="#">立即注册</a>
					<a href="#">找回密码</a>
				</div>
			</div>
    </div>
</template>

<script>
    //import x from ''
    export default {
        name:'Login',
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
//@import url()
#content .login_body{  width:100%;}
.login_body .login_text{ width:100%; height: 40px; border:none; border-bottom: 1px #ccc solid; margin-bottom: 5px; outline: none; text-indent: 10px;}
.login_body .login_btn{ height:50px; margin:10px;}
.login_body .login_btn input{ width:100%; height:100%; background:#e54847; border-radius: 3px; border:none; display: block; color:white; font-size: 20px;}
.login_body .login_link{ display: flex; justify-content:space-between;}
.login_body .login_link a{ text-decoration: none; margin:0 5px; font-size: 12px; color:#e54847;}
</style>