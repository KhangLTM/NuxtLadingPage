<template>
  <div class="bg-white my-6 w-5/6 lg:w-1/4 lg:border-t-2 flex flex-col items-center rounded-t rounded-b-none overflow-hidden shadow-lg ">
      <div class="text-center lg:py-8 py-4 w-full text-5xl text-gray-600 border-b-4"> 
        {{name}}
      </div>
      
      <ul class="w-full text-center ">
        <li class="w-full border-b-2 text-gray-500 py-4 lg:text-gray-700" v-for="(item,index) in list " :key="index">
            {{item}}
        </li>
      </ul>

      <div class="flex items-end py-4 lg:pt-14">
          <h1 class="text-4xl text-gray-700">{{price}}</h1> 
          <p class="text-xl text-gray-700">{{pricePer}}</p>
      </div>
      <button class="mx-auto lg:mx-0 hover:opacity-90 gradient text-white font-bold rounded-full my-6 py-4 px-8 shadow-lg">
          Sign Up
      </button>
  
  </div>
</template>

<script>
import PriceMixin from "./mixin/price"
export default {

  mixins:[PriceMixin]
}
</script>

<style>

</style>