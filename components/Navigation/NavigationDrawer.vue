<template>
 <div>
   <v-app-bar-nav-icon class="d-sm-none" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

   <v-navigation-drawer
     v-model="drawer"
     absolute
     temporary
     right
   >
     <v-list
       nav
       dense
     >
       <v-list-item-group
         v-model="group"
         active-class="deep-purple--text text--accent-4"
       >
         <v-list-item>
           <v-list-item-title>Foo</v-list-item-title>
         </v-list-item>

         <v-list-item>
           <v-list-item-title>Bar</v-list-item-title>
         </v-list-item>

         <v-list-item>
           <v-list-item-title>Fizz</v-list-item-title>
         </v-list-item>

         <v-list-item>
           <v-list-item-title>Buzz</v-list-item-title>
         </v-list-item>
       </v-list-item-group>
     </v-list>
   </v-navigation-drawer>
 </div>
</template>

<script>
export default {
  name: "NavigationDrawer",
  data: () => ({
    drawer: false,
    group: null,
  }),

  watch: {
    group () {
      this.drawer = false
    },
  },
}
</script>

<style scoped>

</style>
