<template>
  <div class="py-8">
    <v-carousel hide-delimiters
                show-arrows-on-hover>
      <v-carousel-item
        reverse-transition="fade-transition"
        transition="fade-transition"
      >
        <div class="slide1 px-4">
          <div
            class="fill-height d-flex flex-column align-center justify-center"
          >
            <div class="slide1-text font-weight-bold">
              پیش ثبت نام آنلاین سال تحصیلی 1401-1402
            </div>
            <br>
            <v-btn nuxt to=""
                   color="color_primary"
                   large
                   class="font-weight-bold">
              ثبت نام
            </v-btn>
          </div>
        </div>
      </v-carousel-item>

      <v-carousel-item
        reverse-transition="fade-transition"
        transition="fade-transition"
      >
        <div class="slide2 px-4">
          <div class="fill-height d-flex flex-column align-center justify-center">
            <div class="slide2-card mx-auto">
              <div class="slide2-title font-weight-bold">
                اطلاعیه
              </div>
              <div class="slide2-text pt-2 font-weight-bold">
                با سلام و احترام به اطلاع می رسانیم سه شنبه مورخ 01/06/1401 کلیه کلاس های تابستانی تعطیل می باشد.
              </div>
            </div>
          </div>
        </div>
      </v-carousel-item>

      <v-carousel-item
        reverse-transition="fade-transition"
        transition="fade-transition"
      >
        <div class="slide3 px-4">
          <div class="fill-height d-flex flex-column align-center justify-center">
            <div class="slide3-card mx-auto">
              <div class="slide3-title font-weight-bold">
                برگزاری آزمون پذیرش میان دوره پایه دوازدهم مدرسه آینده
              </div>
              <div class="slide3-text pt-2 font-weight-bold">
                ثبت نام آزمون میان دوره پایه دوازدهم 1401 - 1402 به صورت هماهنگ و از طریق سامانه ثبت نام استانی انجام می
                شود. ثبت
                نام این آزمون از 30 فروردین ماه آغاز و تا 10 اردیبهشت ماه ادامه خواهد داشت.
                داوطلبان می توانند در تاریخ تعیین شده وارد سایت مدرسه شده و مراحل ثبت نام
                خود را تکمیل نمایند.
              </div>
            </div>
          </div>
        </div>
      </v-carousel-item>

    </v-carousel>
  </div>
</template>

<script>
export default {
  name: "HomeCarousel",
  data() {
    return {}
  },
}
</script>

<style scoped lang="scss">
.slide1 {
  background-image: linear-gradient(rgba(255, 255, 255, .7), rgba(255, 255, 255, .7)), url("assets/Images/Home/backToSchool.jpg");
  background-size: cover;
  width: 100%;
  height: 100%;

  &-text {
    font-size: 30px;
  }
}

.slide2 {
  background-image: linear-gradient(rgba(255, 255, 255, .7), rgba(255, 255, 255, .7)), url("assets/Images/Home/class.jpg");
  background-size: cover;
  width: 100%;
  height: 100%;

  &-card {
    max-width: 380px;
  }

  &-title {
    font-size: 30px;
  }

  &-text {
    font-size: 20px
  }
}

.slide3 {
  background-image: linear-gradient(rgba(255, 255, 255, .7), rgba(255, 255, 255, .7)), url("assets/Images/Home/test.jpg");
  background-size: cover;
  width: 100%;
  height: 100%;

  &-card {
    max-width: 650px;
  }

  &-title {
    font-size: 25px;
  }

  &-text {
    font-size: 20px
  }
}
</style>
