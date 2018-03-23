<template>
    <div>
        <h1>about</h1>
        <p>{{aboutMsg}}</p>
        <h3>我是store数据里面的count2:{{count2}}</h3>
        <router-link to="/"><h1>返回首页面</h1></router-link>
        <router-link to="/home">返回home页面</router-link>
    </div>
</template>
<script>
    export default {
        data () {
            return {
                aboutMsg: '我是about组件',
                count2:this.$store.state.count2
            }
        }
    }
</script>
<style>
    h1{
        color:rgb(156, 56, 56);
    }
</style>
