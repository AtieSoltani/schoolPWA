<template>
  <div>
    <v-footer
      padless
    >
      <v-card
        flat
        tile
        class="footer color_primary darken-3 white--text text-center"
      >
        <v-card-text>
          <v-btn
            v-for="icon in icons"
            :key="icon"
            class="mx-4 white--text"
            icon
          >
            <v-icon size="24px">
              {{ icon }}
            </v-icon>
          </v-btn>
        </v-card-text>

        <div class="d-flex pb-4 px-4 justify-space-between">

          <div class="pr-4 white--text pt-0 d-flex flex-column align-start">
            <div class="footer-title pr-3 pb-2 font-weight-bold text-decoration-underline">دسترسی سریع</div>
            <v-btn v-for="(link, i) in barLinks" :key="i"
                   class="font-weight-bold"
                   nuxt :to="link.route"
                   plain
                   color="white">
              {{ link.title }}
            </v-btn>
          </div>

          <div class="wpr-4 white--text pt-0 d-flex flex-column align-start">
            <div class="footer-title pr-3 pb-2 font-weight-bold text-decoration-underline">ارتباط با مجموعه</div>

            <div class="pb-2 font-weight-bold">
              <v-icon color="white">mdi-map-marker</v-icon>
              همدان، میدان بیمه، 12متری پیروزی، کوچه فتح، مدرسه متوسطه دوم آینده
            </div>

            <div class="pb-2 font-weight-bold">
              <v-icon color="white">mdi-phone</v-icon>
              08138212345
            </div>

            <div class="pb-2 font-weight-bold d-flex">
              <v-icon class="pl-1" color="white">mdi-email</v-icon>
              ayande.school@gmail.com
            </div>
          </div>

          <div class="pl-4 d-none d-md-flex white--text pt-0">
            <iframe class="footer-map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3277.450200195239!2d48.52158280501094!3d34.76944011810888!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3ff1edac9862db19%3A0x84f078133e3530f1!2z2KfYs9iq2KfZhiDZh9mF2K_Yp9mG2Iwg2YfZhdiv2KfZhtiMINqp2YjahtmHINm-24zYsdmI2LLbjNiMINin24zYsdin2YY!5e0!3m2!1sfa!2s!4v1661176150078!5m2!1sfa!2s" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
        </div>

      </v-card>
    </v-footer>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data: () => ({
    icons: [
      'mdi-whatsapp ',
      'mdi-google',
      'mdi-twitter',
      'mdi-instagram',
    ],
    barLinks: [
      {title: 'صفحه اصلی', route: '/'},
      {title: 'گالری تصاویر', route: '/gallery'},
      {title: 'المپیاد و پژوهش', route: '/olympiad-research'},
      {title: 'مشاوره', route: '/'},
      {title: 'افتخارات', route: '/'},
    ],
  }),
}
</script>

<style lang="scss" scoped>
.footer{
  width: 100%;
  &-title {
    font-size: 18px;
    color: black;
  }
  &-map{
    max-width: 300px !important;
    max-height: 230px !important;
  }
}

</style>
