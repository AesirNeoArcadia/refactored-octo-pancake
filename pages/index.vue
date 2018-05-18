<template>
<div>
<section>
  <v-parallax src="banner.png" height="400"  class="elevation-4">
    <v-layout column justify-center align-center >
      <h1>Welcome to Aesir Neo Arcadia.</h1>
      <h3>Don't mind the mess. We're working on it.</h3>
      <p>This site is currently under construction.</p>
    </v-layout>
  </v-parallax>
</section>
<section>
  <v-layout
          column
          wrap
          class="my-5 px-5 mx-5"
          align-center
        >
          <v-flex xs12 sm4 class="my-3">
            <div class="text-xs-center">
              <h2 class="headline">While we're working on this you can still join our servers!</h2>
              <span class="subheading">
                <i>It's <b>HIGHLY RECOMMENDED</b> you subscribe to our <a href="https://steamcommunity.com/sharedfiles/filedetails/?id=1379990767">Mod Collection</a> before connecting!!</i>
              </span>
            </div>
          </v-flex>
          <v-flex xs12>
            <v-container grid-list-xl >
              <v-layout row wrap align-start>
                <v-flex xs12 md4>
                  <v-card class="elevation-4 transparent blue-grey darken-2 fill-height mt-0">
                    <v-card-text class="text-xs-center">
                      <v-icon x-large class="light-blue--text text--lighten-4">fas fa-map</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Maps</div>
                    </v-card-title>
                    <v-card-text class="layout justify-center">
                      <p>Please join us on our stunning collection of ARK maps. We plan to keep a core set of three maps, and have a fourth on rotation. Our current rotation map is Olympus.</p>
                    </v-card-text>
                    <v-list class="blue-grey darken-2">
                      <v-list-tile key="Ragnarok" href='steam://connect/172.103.28.58:27015'>
                        <v-list-tile-content>
                          <v-list-tile-title>Ragnarok</v-list-tile-title>
                        </v-list-tile-content>
                      </v-list-tile>
                      <v-list-tile key="Aberration" href='steam://connect/172.103.28.58:27016'>
                        <v-list-tile-content>
                          <v-list-tile-title>Aberration</v-list-tile-title>
                        </v-list-tile-content>
                      </v-list-tile>
                      <v-list-tile key="The Volcano" href='steam://connect/172.103.28.58:27018'>
                        <v-list-tile-content>
                          <v-list-tile-title>The Volcano</v-list-tile-title>
                        </v-list-tile-content>
                      </v-list-tile>
                      <v-list-tile key="Olympus" href='steam://connect/172.103.28.58:27019'>
                        <v-list-tile-content>
                          <v-list-tile-title>Olympus</v-list-tile-title>
                        </v-list-tile-content>
                      </v-list-tile>
                    </v-list>
                  </v-card>
                </v-flex>
                <v-flex xs12 md4>
                  <v-card class="elevation-4 transparent indigo lighten-1 fill-height mt-0">
                    <v-card-text class="text-xs-center">
                      <v-icon x-large class="light-blue--text text--lighten-4">fab fa-discord</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline">Community</div>
                    </v-card-title>
                    <v-card-text>
                      <p>We are an experienced group of ARK players and server admins who are very excited to bring you this server. We have a strong focus on the community with our 
                      main form of communication being our <a href="https://discord.gg/cnrHUzG" class="blue-grey--text text--lighten-3">Discord server</a> and for status updates and events you can also follow our
                      <a href="https://twitter.com/AesirNeo" class="blue-grey--text text--lighten-3">Twitter</a>.</p>
                      <p>So come and join us in Discord and we'll be happy to greet you and get you involved!</p>
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md4>
                  <v-card class="elevation-4 transparent blue darken-4 fill-height">
                    <v-card-text class="text-xs-center">
                      <v-icon x-large class="light-blue--text text--lighten-4">fas fa-server</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Powerful Server</div>
                    </v-card-title>
                    <v-card-text>
                      <p>Our custom built server is designed to be powerful and stable. We run from an AMD Ryzen 7 2700X CPU, an ASRock X370 Pro4 Motherboard, 32GB of RAM, and dual
                      dedicated 120GB SSDs hosting 2 maps each. We also have additional hard drives for security and backups done daily.</p>
                    </v-card-text>
                  </v-card>
                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
</section>
</div>
</template>
