<template>
  <v-app>
    <v-navigation-drawer
      v-model="drawer"
      app
      right
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
      <v-btn nuxt-link to="/" flat>Home</v-btn>
      <v-btn nuxt-link to="/news" flat>News</v-btn>
      <v-btn nuxt-link to="/server" flat>Server</v-btn>
      <v-btn nuxt-link to="/community" flat>Community</v-btn>
      <v-btn nuxt-link to="/maps" flat>Maps</v-btn>
      <v-btn nuxt-link to="/baseLocations" flat>Base Locations</v-btn>
      <v-btn nuxt-link to="/gallery" flat>Gallery</v-btn>

    </v-toolbar-items>
     <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-toolbar-side-icon>
    </v-toolbar>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
   
    <v-footer :fixed="fixed" app>
      <span>&copy; 2017</span>
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
          { icon: 'bubble_chart', title: 'News', to: '/news' },
          { icon: 'bubble_chart', title: 'Server', to: '/server' },
          { icon: 'bubble_chart', title: 'Community', to: '/community' },
          { icon: 'bubble_chart', title: 'Maps', to: '/maps' },
          { icon: 'bubble_chart', title: 'Base Locations', to: '/baseLocations' },
          { icon: 'bubble_chart', title: 'Gallery', to: '/gallery' }

        ],

        navHome: [
          { to: '/' }
        ],
        miniVariant: false,
        right: true,
        title: 'Aesir Ark Server'
      }
    }
  }
</script>