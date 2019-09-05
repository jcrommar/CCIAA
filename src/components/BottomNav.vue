<template>
  <div class="overflow-hidden">
    <div class="text-center mb-2">
      <v-btn
        text
        color="deep-black"
        @click="showNav = !showNav"
      >
        Siguenos &amp; Comparte
      </v-btn>
    </div>

    <v-bottom-navigation
      :input-value="showNav"
      :value="activeBtn"
      color="blue"
    >
      <v-btn>
        <span>Facebook</span>
        <v-icon>mdi-facebook</v-icon>
      </v-btn>

      <v-btn>
        <span>Instagram</span>
        <v-icon>mdi-instagram</v-icon>
      </v-btn>

      <v-btn>
        <span>Twitter</span>
        <v-icon>mdi-twitter</v-icon>
      </v-btn>
    </v-bottom-navigation>
    <v-footer
      color="black"
      app
    >
      <span class="white--text">Ebenezer Aposento Alto &copy; 2019</span>
    </v-footer>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        activeBtn: 1,
        showNav: true,
      }
    },
  }
</script>