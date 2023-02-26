<template>
    <div class="w-full">

        <h1> Hello ,{{ name }}</h1>
        test
        
        <p>In this series, we will use the following frameworks</p>
        
        </div>      
<br>
        <div>
        <ul>
            <li v-for="framework of frameworks" v-text="framework"></li>
        </ul>
    </div>
</template>


<script>


import AppLayout from '@/Layouts/AppLayout.vue';
export default {
    layout: AppLayout, 
    props: {
        name: String,
        frameworks: Array,
    },
};
</script> 

