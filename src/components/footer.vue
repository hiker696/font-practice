<script setup>
const props = defineProps({
    user:Number,
    url:{
        type: String,
        required: false,
        default:"www.hujiyingcode.com"
    }
})
console.log(props)

</script>

<template>
    <h3>footer</h3>{{  props.user }}

</template>

<style scoped>

</style>