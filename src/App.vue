<script setup>
import { ref ,provide }  from 'vue';
import Header from './components/header.vue';



//响应式数据
const web ={
  name:'hujaiyingnizyuilihai',
  url:'www.hujiying.com'
  
}
provide('provideWeb',web)

const user = ref(0)
provide('provideUser',user)

const userAdd = () => {
  user.value ++
}
provide('provideFuncUserAdd', userAdd)
</script>

<template>
  <h3>App.vue-Top组件</h3>
    user:{{  user }}
  <Header/>

  

</template>

<style scoped>

</style>