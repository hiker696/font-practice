<script setup>
    const emits = defineEmits(['getWeb','userAdd'])
    emits('getWeb',{name:'hujiaying',url:'www.hujiayign.com'})

    const add = () => {
        emits('userAdd',10)
    }
</script>

<template>
    <h3>header</h3>

    <button @click="add">添加用户</button>

</template>

<style scoped>

</style>