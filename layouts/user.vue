<template>
  <v-app>
    <app-bar></app-bar>
    <div class="mt-8"></div>
    <nuxt/>
    <footer-bar></footer-bar>
  </v-app>
</template>

<script>
import AppBar from "~/components/Navigation/AppBar";
import FooterBar from "~/components/Navigation/Footer";

export default {
  name: 'DefaultLayout',
  components: {
    AppBar,
    FooterBar
  },
  data() {
    return {}
  }
}
</script>
