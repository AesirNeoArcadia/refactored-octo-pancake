<template>
<div>
<section>
  <v-parallax src="mapsbg.png" height="350">
    <v-layout column justify-center align-center>
      <h1>Welcome to Aesir Neo Arcadia.</h1>
      <h3>Don't mind the mess. We're working on it.</h3>
      <p>This site is currently under construction.</p>
      <p></p>
    </v-layout>
  </v-parallax>
</section>
<section>
  <v-layout
          column
          wrap
          class="my-5"
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
            <v-container grid-list-xl>
              <v-layout row wrap align-center>
                <v-flex xs12 md4>
                  <v-card class="elevation-0 transparent">
                    <v-card-text class="text-xs-center">
                      <v-icon x-large class="blue--text text--lighten-2">color_lens</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Our Maps</div>
                    </v-card-title>
                    <v-card-text class="layout justify-center">
                      <ul>
                        <li><a href="steam://connect/172.103.28.58:27015">Ragnarok</a></li>
                        <li><a href="steam://connect/172.103.28.58:27016">Aberration</a></li>
                        <li><a href="steam://connect/172.103.28.58:27018">The Volcano</a></li>
                        <li><a href="steam://connect/172.103.28.58:27019">Olympus</a></li>
                    </ul>
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md4>
                  <v-card class="elevation-0 transparent">
                    <v-card-text class="text-xs-center">
                      <v-icon x-large class="blue--text text--lighten-2">flash_on</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline">Community</div>
                    </v-card-title>
                    <v-card-text>
                      We're an experienced bunch of ARK players and server admins who are very excited to bring you this server. We've got a strong focus on the community with our 
                      main form of communication being our <a href="https://discord.gg/cnrHUzG">Discord server</a> and for status updates and events you can also follow our
                      <a href="https://twitter.com/AesirNeo">Twitter</a>.
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md4>
                  <v-card class="elevation-0 transparent">
                    <v-card-text class="text-xs-center">
                      <v-icon x-large class="blue--text text--lighten-2">build</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Powerful Server</div>
                    </v-card-title>
                    <v-card-text>
                      Our custom built server is designed to be powerful and stable. We're running an AMD Ryzen 7 2700X CPU, an ASRock X370 Pro4 Motherboard, 32GB of RAM, and dual
                      dedicated 120GB SSDs hosting 2 maps each. We also have additional hard drives for security and backups done daily.
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
