<template>
    <div>
        <Header />
        <Nuxt />
        <Footer/>
    </div>
</template>

<script>
    import Header from "../components/Header.vue"
    import Footer from "../components/Footer.vue"

export default {
    components:{
        Header,
        Footer
    }    
}
</script>
<style>
  
  *{
     margin:0;
    padding:0;
  }
  html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  overflow-x: hidden;
  font-size: 16px;
  word-spacing: 1px;
  min-height: 1000px;
  scroll-behavior: smooth;  
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background: linear-gradient(90deg, #d53369 0%, #daae51 100%);
} 

.gradient2{
     background: linear-gradient(90deg, #d53369 0%, #db8515 100%);
}

.gradient {
  /* background: linear-gradient(90deg, #6200ee 0%, #03dac5 100%);  */
  background: linear-gradient(90deg, #d53369 0%, #daae51 100%);
}
</style>
</style>