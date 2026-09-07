<script setup>
    import { ref } from 'vue'

    // Add code here
    import image from '../../public/assets/me.png'

    //multiple attribute binding
    const obj = ref({
        src:'/assets/me.png',
        width: "200",
        height: "200"
    })
</script>

<template>

    <!-- Add code here -->
   <h1>
    <img v-bind:src="image" :width="200" :height="200"><hr>
   </h1>

   <img v-bind:src="obj">
</template>
