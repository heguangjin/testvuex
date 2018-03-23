<template>
    <div>
        <h1>home:{{count}}</h1>
        <p>{{msg}}</p>
        <router-link to="/">返回首页面</router-link>
        <router-link to="/about">返回about页面</router-link>
        <child11></child11>
    </div>
</template>

<script>
import child3 from './child3.vue'
    export default {
        data () {
            return {
                msg: "我是home 组件",
                count:this.$store.getters.getCount
            }
        },
        components:{
            child11:child3
        }
    }
</script>