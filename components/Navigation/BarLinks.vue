<template>
  <div class="d-none d-sm-block">
    <v-btn v-for="(link, i) in barSimpleLinks" :key="i"
           nuxt :to="link.route"
           plain>
      {{ link.title }}
    </v-btn>

    <v-menu
      open-on-hover
      offset-y
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          text
          v-bind="attrs"
          v-on="on"
        >
          درباره ما
          <v-icon class="mr-1" size="small">mdi-chevron-down</v-icon>
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="(item, index) in items"
          :key="index"
        >
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>

  </div>
</template>

<script>
export default {
  name: "BarLinks",
  data: () => ({
    barSimpleLinks: [
      {title: 'صفحه اصلی', route: '/'},
      {title: 'گالری تصاویر', route: '/'},
      {title: 'المپیاد و پژوهش', route: '/'},
      {title: 'مشاوره', route: '/'},
      {title: 'افتخارات', route: '/'},
    ],
    items: [
      { title: 'Click Me' },
      { title: 'Click Me' },
      { title: 'Click Me' },
      { title: 'Click Me 2' },
    ],
  }),
}
</script>

<style scoped>

</style>
