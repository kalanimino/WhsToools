<template>
    <v-container class="grey lighten-3">

        <v-layout row justify-start wrap>

            <v-flex xs12 md6>
                
                <v-container column>

                    <v-flex xs12>
                        <p class="display-1">About PHN</p>
                    </v-flex>

                    <v-flex xs12>
                        <p class="headline">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fuga obcaecati qui doloremque enim soluta tenetur cum esse dolorem quas libero voluptatibus est eligendi cumque saepe quia, eveniet aliquam consectetur odit!</p>
                    </v-flex>

                </v-container>

            </v-flex>

            <v-flex xs12 md6>
                <v-responsive>
                    <v-img :src="require('@/assets/homepage/template3.jpg')" :apect-ratio="16/9" max-height="300" contain></v-img>
                </v-responsive>
            </v-flex>

        </v-layout>

    </v-container>
</template>

<script>
  export default {
    data: () => ({

    })
  }
</script>
