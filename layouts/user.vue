<template>
  <v-app>
    <app-bar></app-bar>
    <div class="mt-8"></div>
    <Nuxt/>

  </v-app>
</template>

<script>
import AppBar from "~/components/Navigation/AppBar";

export default {
  name: 'DefaultLayout',
  components: {
    AppBar
  },
  data() {
    return {}
  }
}
</script>
