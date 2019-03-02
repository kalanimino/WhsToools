<template>
  <v-layout justify-center row wrap>
      <v-btn v-for="link in links" :key="link" color="grey" flat round>
        {{ link }}
      </v-btn>
      <v-btn color="grey" flat round>
        <v-icon>code</v-icon>
      </v-btn>

      <v-flex grey lighten-3 py-3 text-xs-center grey--text xs12 >
        <strong>Waipahu High School</strong>
      </v-flex>
    </v-layout>
</template>

<script>
  export default {
    data: () => ({
      links: [
          'About',
          'Contact Us',
      ]

    })
  }
</script>
