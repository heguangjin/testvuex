<template>
  <div>
      <h3>我是子组件的子组件child3:{{$store.state.count}}</h3>
      <child12></child12>
  </div>

</template>
<script>
import aboutchild from './about.vue'
export default {
  data(){
      return {}
  },
  components:{
    child12:aboutchild
 }
}
</script>
