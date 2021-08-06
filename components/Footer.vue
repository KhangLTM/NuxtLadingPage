<template>
    <div class="w-full bg-white"  >
        <div class=" flex flex-col lg:flex-row">    
            <div class=" my-5 ml-4 lg:w-1/5 lg:flex items-center justify-center">
                <logo class="text-red-500"/>
            </div>
            <div class=" lg:flex  lg:flex-grow  items-center justify-center ml-4 leading-10 pb-10 ">
                <div class="w-full lg:w-1/4">
                    <h1 class="lg:py-10 text-gray-500 text-xl">Actions</h1>
                    <ul class=" w-1/2 lg:block flex justify-around ">
                        <li>LINK</li>
                        <li>LINK</li>
                        <li>LINK</li>
                    </ul>
                </div>
                <div class="lg:w-1/4">
                    <h1 class="lg:py-10 text-gray-500 text-xl">Actions</h1>
                    <ul class=" w-1/2 lg:block flex justify-around ">
                        <li>LINK</li>
                        <li>LINK</li>
                        <li>LINK</li>
                    </ul>
                </div>
                <div class="lg:w-1/4">
                    <h1 class="lg:py-10 text-gray-500 text-xl">Actions</h1>
                    <ul class=" w-1/2 lg:block flex justify-around ">
                        <li>LINK</li>
                        <li>LINK</li>
                        <li>LINK</li>
                    </ul>
                </div>
                <div class="lg:w-1/4">
                    <h1 class="lg:py-10 text-gray-500 text-xl"  >Actions</h1>
                    <ul class=" w-1/2 lg:block flex justify-around ">
                        <li>LINK</li>
                        <li>LINK</li>
                        <li>LINK</li>
                    </ul>
                </div>
            
            
            </div>
        
        </div>
    </div>
</template>



<script>

import Logo from "./Logo.vue"


export default {
    components:{
        Logo,
    }
}
</script>

<style>

</style>