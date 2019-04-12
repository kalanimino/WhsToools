<template>
  <div class="HeaderCom">
    <v-toolbar fixed app class="">
      <v-toolbar-side-icon @click="drawer=!drawer"></v-toolbar-side-icon>
      <v-toolbar-title class="headline text-uppercase mr-5">
        <span>PHN</span>
        <span class="subheading font-weight-light "> WHS TOOLS</span>
      </v-toolbar-title>

      <v-toolbar-items>

        <v-btn flat color="grey" class="" href="@/App">
          <v-icon>home</v-icon>
        </v-btn>

        <v-menu offset-y open-on-hover>
          <template v-slot:activator="{ on }">
          <v-btn flat color="grey" class="px-4" v-on="on">
            <span>Registration</span>
          </v-btn>
          </template>
        <v-list>
          <v-list-tile v-for="menu in menu" :key="menu" @click="">
            <v-list-tile-title>{{ menu.title }}</v-list-tile-title>
          </v-list-tile>
        </v-list>
        </v-menu>
        <v-divider vertical class="py-3" inset></v-divider>
        
        <v-menu offset-y open-on-hover>
          <template v-slot:activator="{ on }">
          <v-btn flat color="grey" v-on="on">
          <span>Honors</span>
          </v-btn>
          </template>
        <v-list>
          <v-list-tile v-for="menu in menu2" :key="menu" @click="">
            <v-list-tile-title>{{ menu.title }}</v-list-tile-title>
          </v-list-tile>
        </v-list>
        </v-menu>
       
      </v-toolbar-items>

      <v-spacer></v-spacer>

      <v-toolbar-items>
        <v-text-field label="Search..." prepend-icon="search" class="mr-3"></v-text-field>
      </v-toolbar-items>
    </v-toolbar>
    <v-navigation-drawer v-model="drawer" color="red" app></v-navigation-drawer>
  </div>
</template>

<script>
  export default {
    data: () => ({
      drawer: false,
      menu: [
        {title:"registration", icon: "some_Icon", link:"some_link"},
        {title:"registration", icon: "some_Icon", link:"some_link"},
        {title:"registration", icon: "some_Icon", link:"some_link"},
        {title:"registration", icon: "some_Icon", link:"some_link"}
      ],

      menu2: [
        {title:"honors", icon: "some_Icon", link:"some_link"},
        {title:"honors", icon: "some_Icon", link:"some_link"},
        {title:"honors", icon: "some_Icon", link:"some_link"},
        {title:"honors", icon: "some_Icon", link:"some_link"}
      ]

    })
  }
</script>
