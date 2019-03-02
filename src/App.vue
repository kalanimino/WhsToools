<template>
  <v-app>
    <v-content class="grey lighten-4">
      <Header/>
    </v-content>
    <v-footer class="grey lighten-2" height="auto">
    <Footer/>
    </v-footer>
  </v-app>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'
export default {
  name: 'App',
  components: {
    Header,
    Footer
  },
  data () {
    return {
      //
    }  
  }
}
</script>
