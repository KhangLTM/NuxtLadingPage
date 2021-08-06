<template>
  <div class=" bg-white w-5/6  lg:w-1/5 my-5 flex flex-col items-center rounded-t rounded-b-none overflow-hidden shadow">
      <div class="text-center py-4 w-full text-4xl text-gray-900 border-b-4 lg:text-gray-500"> 
        {{name}}
      </div>
      
      <ul class="w-full text-center ">
        <li class="w-full border-b-2 text-gray-500 py-4 lg:py-2" v-for="(item,index) in list " :key="index">
            {{item}}
        </li>
      </ul>

      <div class="flex items-end py-4 ">
          <h1 class="text-4xl text-gray-700 lg:tex-gray-500">{{price}}</h1> 
          <p class="text-xl text-gray-600 lg:text-gray-500">{{pricePer}}</p>
      </div>
      <button class="lg:opacity-90 mx-auto lg:mx-0 hover:opacity-90 gradient text-white font-bold rounded-full my-6 py-4 px-8 shadow-lg">
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