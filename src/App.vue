<template>
  <v-app>
    
    <v-content id="body" class="grey lighten-4">
      <Banner/>
      <Home/>
    </v-content>

  </v-app>
</template>

<script>
import Home from '@/Home'
import Banner from '@/components/Banner'
export default {
  name: 'App',
  components: {
    Home,
    Banner
  },
  data () {
    return {
      //
    }  
  }
}
</script>
