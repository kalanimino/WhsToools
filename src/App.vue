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

<style>
a{
  text-decoration: none
}
</style>
<<<<<<< HEAD

=======
>>>>>>> 452d4f5e9e00ac4a430dd0b576f8857e448dcc4c
