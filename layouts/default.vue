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
            <v-list-tile-title v-text="item.title" class="sitetitle"></v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar fixed app>
         
      <v-toolbar-title router
          :to="navHome.to" v-text="title" class="sitetitle"></v-toolbar-title>
    
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
      <v-btn nuxt-link to="/" flat><v-icon small left>fas fa-home</v-icon>Home</v-btn>
      <v-btn nuxt-link to="/#" flat><v-icon small left>fas fa-info</v-icon>Server Info</v-btn>
      <v-btn nuxt-link to="/#" flat><v-icon small left>fas fa-map</v-icon>Maps</v-btn>
      <v-btn nuxt-link to="/#" flat><v-icon small left>fas fa-images</v-icon>Gallery</v-btn>
      <v-btn href="https://discord.gg/cnrHUzG" flat><v-icon small left>fab fa-discord</v-icon>Discord</v-btn>
      <v-btn nuxt-link to="/#" flat><v-icon small left>fas fa-question-circle</v-icon>About</v-btn>

    </v-toolbar-items>
     <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-toolbar-side-icon>
    </v-toolbar>
    <v-content>
      <nuxt />
    </v-content>
   
    <v-footer :fixed="fixed" app>
      <span>&copy; 2018 Aesir Neo Arcadia</span>
      <v-spacer></v-spacer>
      <span align-center class="pr-4 pt-1">
        <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
          <input type="hidden" name="cmd" value="_s-xclick">
          <input type="hidden" name="hosted_button_id" value="ZACLWXJP2UAH2">
          <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
          <img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
        </form>
      </span>
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
          { icon: 'fas fa-home', title: 'Home', to: '/' },
          { icon: 'fas fa-info', title: 'Server Info', to: '/#' },
          { icon: 'fas fa-map', title: 'Maps', to: '/#' },
          { icon: 'fas fa-images', title: 'Gallery', to: '/#' },
          { icon: 'fas fa-question-circle', title: 'About', to: '/#' }
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
<style>
  .sitetitle {
    font-family: 'Cabin Condensed';
    
  }
</style>