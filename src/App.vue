<script setup>
import { reactive, ref }  from 'vue';
import Header from './components/header.vue';



//响应式数据
const web = reactive({
  name:'hujaiyingnizyuilihai',
  url:'www.hujiying.com'
  
})

const user = ref(0)

const emitsGetWeb = (data) =>{
  console.log(data)
  web.url = data.url
}

const emitsUserAdd = (data) => {
  console.log(data)
  user.value += data
}
</script>

<template>
  <Header @getWeb="emitsGetWeb" @userAdd="emitsUserAdd"/>

  {{ web.url }} -{{ user }}

</template>

<style scoped>

</style>