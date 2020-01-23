<template>
  <v-app>
    <Navigation/>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-avatar>
          <v-img
            alt="UFDO Logo"
            class="shrink mr-2"
            contain
            src="../src/assets/logo.jpg"
            transition="scale-transition"
            width="40"
          />
        </v-avatar>

        <!-- <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        /> -->
        <span>Ua Fandub Open Chat Announcements</span>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://t.me/ua_fundub_open"
        target="_blank"
        text
      >
        <span class="mr-2">Chat</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>
    <v-content>
      <!-- <HelloWorld/> -->
      <announsment/>
    </v-content>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld'
import announsment from './components/announsment'
import Navigation from './components/Navigaton'

export default {
  name: 'App',

  components: {
    // HelloWorld,
    announsment,
    Navigation
  },

  data: () => ({
    //
  })
}
</script>
