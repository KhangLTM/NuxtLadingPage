<template>
  <div class="bg-gray-100 flex flex-col lg:flex-row  items-center justify-center bg-white py-5">
      <price name="Free" price="0$" :limited="true" :list="listFree" />
      <hilighted-price name="Basic" price="0$" :limited="true" :list="listBasic" />
      <price name="Pro" price="0$" :limited="true" :list="listPro"/>
  </div>
</template>

<script>

import Price from "./Price.vue"
import HilightedPrice from "./HilightedPrice.vue"

export default {
    data() {
    return {
      listFree: ['Thing', 'Thing', 'Thing'],
      listBasic: ['Thing', 'Thing', 'Thing', 'Thing'],
      listPro: ['Thing', 'Thing', 'Thing', 'Thing', 'Thing']
    }
  },
    components:{HilightedPrice,Price}
}
</script>

