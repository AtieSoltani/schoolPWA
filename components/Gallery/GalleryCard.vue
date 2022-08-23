<template>
  <div class="elevation-3 pa-2 mx-2 mb-8 mt-4 rounded-xl">
    <p class="text-center font-weight-bold text-decoration-underline">
      {{title}}
    </p>
    <v-row>
      <v-col
        v-for="(img ,i) in img"
        :key="i"
        class="d-flex child-flex"
        cols="4"
      >
        <v-img
          :src="require(`@/assets/Images/Gallery/1/${img}`)"
          :lazy-src="require(`@/assets/Images/Gallery/1/${img}`)"
          aspect-ratio="1"
          class="grey lighten-2 rounded-xl"
        >
          <template v-slot:placeholder>
            <v-row
              class="fill-height ma-0"
              align="center"
              justify="center"
            >
              <v-progress-circular
                indeterminate
                color="grey lighten-5"
              ></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "GalleryCard",
  props:{
    img:[],
    title:""
  }
}
</script>

<style scoped>

</style>
