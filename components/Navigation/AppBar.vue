<template>
  <div class="mb-16 overflow-hidden">
    <v-app-bar
      fixed
      color="#6babfb"
      shrink-on-scroll
      src="https://cdn-res.keymedia.com/cms/images/au/130/0314_637375358083115310.jpg"
      fade-img-on-scroll
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(107, 171, 251,.9), rgba(203, 235, 255,.9)"
        ></v-img>
      </template>

      <navigation-drawer/>

      <v-app-bar-title class="font-weight-black">
        <span class="bar-title">مدرسه آینده</span>
      </v-app-bar-title>

      <v-spacer></v-spacer>
      <img src="@/assets/Images/logo.png"
           class="mt-2"
           height="60"
           width="60">

      <template v-slot:extension>
        <BarLinks/>
        </template>
    </v-app-bar>
  </div>

</template>

<script>
import NavigationDrawer from "~/components/Navigation/NavigationDrawer";
import BarLinks from "~/components/Navigation/BarLinks";
export default {
  name: "AppBar",
  components: {
    NavigationDrawer,
    BarLinks
  },
  data() {
    return {}
  }
}
</script>

<style lang="scss" scoped>
.bar-title{
  font-size: 20px !important;

}
</style>
