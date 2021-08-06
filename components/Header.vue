<template>
  <nav      
  :class="headerClasslist "
  class=" flex  lg:justify-around z-999999 sticky top-0 w-full lg:border-double lg:border-b-4 border-b-2 ">
      <div 
      class="lg:py-3  flex flex-wrap  w-full lg:flex lg:flex-row lg:items-center  justify-between ">
            <div>
                <logo 
                :class="logoClasslist"
                class="mt-5  lg:ml-5"/>
            </div>
            <div class=" items-center flex items-center flex-row-reverse ralative lg:hidden">
                <button
                    @click="clickToggle"
                >
                    <svg
                    class="fill-current h-6 w-6"
                    viewBox="0 0 20 20"
                    xmlns="http://www.w3.org/2000/svg"
                    >
                    <title>Menu</title>
                    <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
                    </svg>
                
                </button>

            
            </div>
            
            <div 
                v-show="Toggle"
                class=" w-full lg:w-1/5  z-99"
                >
                <ul
                    :class="logoClasslist"
                    class="leading-8 lg:leading-4 w-full absolute top-9 lg:-top-2 flex flex-col  lg:flex-row lg:px-10 items-center  py-4 bg-gray-200 lg:bg-transparent"
                >
                    <li class="mr-3">LINK</li>
                    <li class="mr-3">LINK</li>
                    <li class="mr-3">LINK</li>
                    <li class="mr-3">
                        <button
                            class="gradient2 lg:mx-0 hover:bg-gray-200 font-bold rounded-full mt-4 lg:mt-0 py-4 px-8 shadow "
                        >ACTION</button></li>
                </ul>
            </div>

      
      </div>
  </nav>
</template>



<script>
    import Logo from './Logo.vue'

export default {
    components:{
        Logo,
    },
    data(){
        return{
            scrollY:0,
            Toggle:false,
        }
    },
   
  computed:{
      isSticky(){
          return this.scrollY >10
      },
      
      headerClasslist(){
          return this.isSticky ? 'bg-white opacity-80 shadow' : 'gradient' 
      },

     logoClasslist(){
         return this.isSticky ? 'text-black' : 'text-white'
     }   
  
  },
    mounted(){
    this.scrollY = window.scrollY
    document.addEventListener('scroll', this.onScroll)
    window.addEventListener('resize',this.setNavOpen())
    },
  
  methods:{

        onScroll(){
            this.scrollY= window.scrollY
        },
        
        setNavOpen(){
            const {width}=window.screen  
            if(width > 820) this.Toggle=true
        },
        clickToggle(){
            this.Toggle=!this.Toggle
        }
    },




}
</script>

<style>

</style>