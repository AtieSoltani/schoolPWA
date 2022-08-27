<template>
 <div>

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
         active-class="deep-purple--text text--accent-4">


         <v-list-item
           v-for="(link, index) in barSimpleLinks"
           :key="index"
         >
           <v-list-item-title>
             <v-btn nuxt :to="link.route"
                    class="font-weight-bold"
                    plain>
               {{ link.title }}
             </v-btn>
           </v-list-item-title>
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
    drawer: true,
    group: null,
    barSimpleLinks: [
      {title: 'صفحه اصلی', route: '/'},
      {title: 'گالری تصاویر', route: '/gallery'},
      {title: 'المپیاد و پژوهش', route: '/olympiad-research'},
      {title: 'مشاوره', route: '/consultation'},
      {title: 'افتخارات', route: '/error'},
      {title: 'تماس با ما', route: ""},
      {title: 'اهداف و چشم انداز مدرسه', route: ""},
      {title: 'تاریخچه مدرسه آینده', route: ""},
      {title: 'همکاران ما', route: ""},
      {title: 'آرشیو خبرها', route: "/news-archive"},
      {title: 'اطلاعیه ها', route: ""},
      {title: 'پربازدید ترین اخبار', route: ""},
      {title: 'رویداد ها', route: ""},

    ],
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
