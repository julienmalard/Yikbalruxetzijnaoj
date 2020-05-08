<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      :src="require('./assets/ruwi.jpg')"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="./assets/logo.svg"
          transition="scale-transition"
          width="50"
        />

        <v-toolbar-title>Ruxe'el tzij Atitya'</v-toolbar-title>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/julienmalard/yikbalruxetzijnaoj"
        target="_blank"
        text
      >
        <span class="mr-2">GitHub</span>
        <v-icon>mdi-github</v-icon>
      </v-btn>
    </v-app-bar>

    <v-content>
    <v-container id="create">
      <v-speed-dial
      v-model="fab"
      top
      left
      direction="bottom"
      transition="slide-y-transition"
    >

      <template v-slot:activator>
        <v-btn
          v-model="fab"
          color="white"
          fab
        >
          <v-icon black v-if="fab">mdi-close</v-icon>
          <v-icon black v-else>mdi-dots-horizontal</v-icon>
        </v-btn>
      </template>
       <v-btn
        fab
        small
        color="white"
      >
        <v-icon>mdi-pencil</v-icon>
      </v-btn>
      <v-btn
        fab
        small
        color="white"
      >
        <v-icon>mdi-plus</v-icon>
      </v-btn>
      <v-btn
        fab
        small
        color="white"
      >
        <v-icon>mdi-translate</v-icon>
      </v-btn>
    </v-speed-dial>
    <Rukuux/>
    </v-container>
    </v-content>

  </v-app>
</template>

<script>
import Rukuux from './components/Rukuux';

export default {
  name: 'App',

  components: {
    Rukuux,
  },

  data: () => ({
    fab: false
  }),
};
</script>

<style scoped>
  /* This is for documentation purposes and will not be needed in your application */
  #create .v-speed-dial {
    position: absolute;
  }

  #create .v-btn--floating {
    position: relative;
  }
</style>