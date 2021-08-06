<template>
    <div>
        <scroll-to-top />
        <hero/>
        <feature/>
        <teasers />
        <prices />
        <call-to-action/>
    </div>
</template>

<script>
import Hero from '../components/Hero.vue'
import Feature from "../components/Feature.vue"
import Teasers from '../components/Teasers.vue'
import Prices from '../components/prices.vue'
import CallToAction from '../components/CallToAction.vue'
import ScrollToTop from '../components/SrollToTop.vue'
export default {
  components: { Hero,Feature,Teasers,Prices,CallToAction,ScrollToTop }
}
</script>
