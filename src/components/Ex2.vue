<script setup>
    import { ref } from 'vue'

    // Add code here
    const width = ref('200')
    const height = ref('200')
    const myImg = ref('../../public/assets/me.png')

    //multiple attribute binding
    const obj = ref({
        src:"../../public/assets/me.png" ,
        width: "200" ,
        height: "200"
    })
</script>
<template>

    <!-- Add code here -->
    <img v-bind:src="myImg" :width="width" :height="height">
    <img v-bind=obj>
</template>
