<template>
  <div
    :class="classList"
    class="lg:mx-10 lg:mt-14 mt-4 flex flex-col items-center rounded-t rounded-b-none shadow-md"
    >
      <div class="lg:py-10 w-80 leading-7 ">
        <h2 class="text-gray-500"><slot name="overline"></slot></h2>
        <p class="text-xl"><slot name="headline"></slot></p>
        <p><slot name="content"></slot></p>
      </div>
      <div>
        <button
          class="mx-auto lg:mx-0 hover:opacity-80 cursor-pointer gradient text-white font-bold rounded-full my-6 py-4 px-8 shadow-lg"
        
        >{{action}}</button>

      </div>

  </div>
</template>

<script>
export default {
  props:{
    action:{
      type:String,
      require:true
    },
    rows:{
      type:Number,
      require:true,  
      validator:value=>{
        return value > 1 && value <=6
        }
    }
  },
  computed:{
    classList(){
      return `md:w-1/${this.rows}`
    }
  }
  
  
  
  }

</script>

<style>

</style>