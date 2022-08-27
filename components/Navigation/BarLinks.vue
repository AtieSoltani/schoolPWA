<template>
  <div class="d-none d-sm-block">
    <v-btn v-for="(link, i) in barSimpleLinks" :key="i"
           nuxt :to="link.route"
           class="font-weight-bold"
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
          class="font-weight-bold">
          اخبار
          <v-icon class="mr-1" size="small">mdi-chevron-down</v-icon>
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="(NewsItem, index) in newsDropdown"
          :key="index"
          class="font-weight-bold">
          <v-list-item-title>
            <v-btn nuxt :to="NewsItem.route"
                   class="font-weight-bold"
                   plain>
              {{ NewsItem.title }}
            </v-btn>
          </v-list-item-title>

        </v-list-item>
      </v-list>
    </v-menu>

    <v-menu
      open-on-hover
      offset-y
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          text
          v-bind="attrs"
          v-on="on"
          class="font-weight-bold">
          درباره ما
          <v-icon class="mr-1" size="small">mdi-chevron-down</v-icon>
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="(UsItem, index) in usDropdown"
          :key="index"
        >
          <v-list-item-title>
            <v-btn nuxt :to="UsItem.route"
                   class="font-weight-bold"
                   plain>
              {{ UsItem.title }}
            </v-btn>
          </v-list-item-title>
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
      {title: 'گالری تصاویر', route: '/gallery'},
      {title: 'المپیاد و پژوهش', route: '/olympiad-research'},
      {title: 'مشاوره', route: '/consultation'},
      {title: 'افتخارات', route: '/error'},
    ],
    usDropdown: [
      {title: 'تماس با ما', route: ""},
      {title: 'اهداف و چشم انداز مدرسه', route: ""},
      {title: 'تاریخچه مدرسه آینده', route: ""},
      {title: 'همکاران ما', route: ""},
    ],

    newsDropdown: [
      {title: 'آرشیو خبرها', route: "/news-archive"},
      {title: 'اطلاعیه ها', route: ""},
      {title: 'پربازدید ترین اخبار', route: ""},
      {title: 'رویداد ها', route: ""},
    ],
  }),
}
</script>

<style scoped>

</style>
