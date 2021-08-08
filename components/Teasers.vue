<template>
    <div class="flex flex-col  items-center bg-white py-5">
        
             <div>
                <h1 class="text-5xl text-gray-700">Title</h1>
             </div>
            <div class="lg:w-1/6 w-1/3 gradient py-0.5">
            </div>
            
            <div class=" lg:flex lg:flex-row lg:justify-center">
                <teasers-col data-aos="zoom-in"  data-aos-delay="400" data-aos-offset="100" :rows="3" action="Action"
                >
                     <template #overline>GETTING STARTED</template>
                     <template #headline>Lorem ipsum dolor sit amet</template>
                     <template #content>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam at
                            ipsum eu nunc commodo posuere et sit amet ligula.</template>

                </teasers-col>    
                <teasers-col  data-aos="zoom-in"  data-aos-delay="400" data-aos-offset="200" :rows="3" action="Action"
                >
                     <template #overline>GETTING STARTED</template>
                     <template #headline>Lorem ipsum dolor sit amet</template>
                     <template #content>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam at
                            ipsum eu nunc commodo posuere et sit amet ligula.</template>

                </teasers-col>    
                <teasers-col data-aos="zoom-in"  data-aos-delay="400" data-aos-offset="300" :rows="3" action="Action"
                >
                     <template #overline>GETTING STARTED</template>
                     <template #headline>Lorem ipsum dolor sit amet</template>
                     <template #content>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam at
                            ipsum eu nunc commodo posuere et sit amet ligula.</template>

                </teasers-col>        
            
            
            </div>
        
    



    </div>
</template>

<script>

import TeasersCol from "./TeasersCol.vue" 


export default {
    components:{
        TeasersCol,
    }
}
</script>

<style>

</style>
