<template>
  <v-app>
      <v-card
    color="grey lighten-5"
    flat
    height="100px"
    tile
  >
      <v-toolbar dense>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Bourbons</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
    </v-toolbar>
      </v-card>

    <v-content>
      <HelloWorld/>
    </v-content>

  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data: () => ({
     extended: false,
      extendedSlot: false,
      prominent: false,
      dense: true,
      collapse: false,
      flat: false,
      bg: false,
      extensionHeight: 48,
  }),
};
</script>
