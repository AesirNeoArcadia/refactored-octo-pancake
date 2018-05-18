<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      app
      right
      class="grey darken-4"
    >
      <v-list>
        <v-list-tile
          router
          :to="item.to"
          :key="i"
          v-for="(item, i) in items"
          exact
        >
          <v-list-tile-action>
            <v-icon v-html="item.icon"></v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title v-text="item.title"></v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar fixed app>
         
      <v-toolbar-title router
          :to="navHome.to" v-text="title"></v-toolbar-title>
    
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
      <v-btn nuxt-link to="/#" flat>Home</v-btn>
      <v-btn nuxt-link to="/#" flat>Server Info</v-btn>
      <v-btn nuxt-link to="/#" flat>Maps</v-btn>
      <v-btn nuxt-link to="/#" flat>Gallery</v-btn>
      <v-btn href="https://discord.gg/cnrHUzG" flat>Discord</v-btn>
      <v-btn nuxt-link to="/#" flat>About</v-btn>

    </v-toolbar-items>
     <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-toolbar-side-icon>
    </v-toolbar>
    <v-content>
      <nuxt />
    </v-content>
   
    <v-footer :fixed="fixed" app>
      <span>&copy; 2018 Aesir Neo Arcadia</span>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: false,
        fixed: false,
        items: [
          { icon: 'apps', title: 'Home', to: '/' },
          { icon: 'bubble_chart', title: 'Server Info', to: '/#' },
          { icon: 'bubble_chart', title: 'Maps', to: '/#' },
          { icon: 'bubble_chart', title: 'Gallery', to: '/#' },
          { icon: 'bubble_chart', title: 'About', to: '/#' }

        ],

        navHome: [
          { to: '/' }
        ],
        miniVariant: false,
        right: true,
        title: 'Aesir Neo Arcadia'
      }
    }
  }
</script>