<template>
    <div class="w-full">

        <h1> Hello ,{{ name }}</h1>
        test
        
        <p>In this series, we will use the following frameworks</p>
        

        <button class="bg-blue-400 2xl:bg-green-500 py-2  px-10 hover:bg-green-400 font-bold hover:font-thin xs:">Submit</button>
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

