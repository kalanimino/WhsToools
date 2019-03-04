<template>
  <v-app>
    
    <v-content id="body" class="grey lighten-4">
      <Header/>
      <Banner/>
      <Cards/>
      <About/>
    </v-content>

    <Footer/> 

  </v-app>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'
import Banner from '@/components/Banner'
import Cards from '@/components/Cards'
import About from '@/components/About'
export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Banner,
    Cards,
    About
  },
  data () {
    return {
      //
    }  
  }
}
</script>
