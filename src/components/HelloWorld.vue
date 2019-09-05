<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <v-list dense>
        // eslint-disable-next-line
        <v-list-item @click="">
          <v-list-item-action>
            <v-icon>mdi-home</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Inicio</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        // eslint-disable-next-line
        <v-list-item @click="">
          <v-list-item-action>
            <v-icon>mdi-shield-outline</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Cobertura</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        // eslint-disable-next-line
        <v-list-item @click="">
          <v-list-item-action>
            <v-icon>mdi-account-multiple</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Pastores</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        // eslint-disable-next-line
        <v-list-item @click="">
          <v-list-item-action>
            <v-icon>mdi-library-video</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Presentaciones</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        // eslint-disable-next-line
        <v-list-item @click="">
          <v-list-item-action>
            <v-icon>mdi-video</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Videos</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        // eslint-disable-next-line
        <v-list-item @click="">
          <v-list-item-action>
            <v-icon>mdi-book</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Revista Rhema</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        // eslint-disable-next-line
        <v-list-item @click="">
          <v-list-item-action>
            <v-icon>mdi-contact-mail</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Contact</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      app
      color="black"
      dark
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title class="headline text-uppercase">
        <span>Ebenezer </span>
        <span class="font-weight-light">Aposento Alto</span>
      </v-toolbar-title>
      <div class="flex-grow-1"></div>
      <v-btn icon>
        <v-icon>mdi-facebook</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-instagram</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-twitter</v-icon>
      </v-btn>
    </v-app-bar>
  </v-app>
</template>

<script>
  export default {
    props: {
      source: String,
    },
    data: () => ({
      drawer: false,
    }),
  }
</script>