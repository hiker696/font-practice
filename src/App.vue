<script setup>
import Header from './components/header.vue'
import Footer from './components/footer.vue'

</script>

<template>
  <h3>App.vue</h3>

  <Header>
    <a href="dengruicode.com">胡家瑛你是最棒的</a>
  </Header>

  <Footer>
    <!-- <template v-slot:url> -->
    <template #url>
    <a href="dengruicode.com">网址</a>
    </template>
  </Footer>

</template>

<style scoped>

</style>