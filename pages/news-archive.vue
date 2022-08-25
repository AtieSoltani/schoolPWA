<template>
  <div class="mt-16">
    <div class="mt-16">
      <br>
      <div class="news ma-md-8 mx-2 font-weight-black d-flex align-center justify-center">
        آرشیو خبرها
      </div>
      <div class="pa-4 d-sm-flex rounded-lg justify-space-around">

        <div>
          <v-card v-for="(news , i) in news1" :key="i"
                  class="mx-auto my-12"
                  max-width="374"
          >
            <template slot="progress">
              <v-progress-linear
                color="deep-purple"
                height="10"
                indeterminate
              ></v-progress-linear>
            </template>

            <v-img
              height="250"
              :src="require(`@/assets/Images/Home/LatestNews/${news.img}`)"
            ></v-img>

            <div>
              <v-btn nuxt to=""
                     color="color_primary"
                     class="font-weight-bold"
                     text>
                {{ news.title }}
              </v-btn>
            </div>

            <v-card-text>

              <div class="mb-2 text-subtitle-1">
                <div class="latest-news-date pt-4"><span class="gray--text pr-2">{{ news.time }}</span>{{ news.date }}
                </div>
              </div>

              <div>
                {{ news.description }}
              </div>
            </v-card-text>
          </v-card>
        </div>

        <div>
          <v-card v-for="(news , i) in news2" :key="i"
                  class="mx-auto my-12"
                  max-width="374"
          >
            <template slot="progress">
              <v-progress-linear
                color="deep-purple"
                height="10"
                indeterminate
              ></v-progress-linear>
            </template>

            <v-img
              height="250"
              :src="require(`@/assets/Images/Home/LatestNews/${news.img}`)"
            ></v-img>

            <div>
              <v-btn nuxt to=""
                     color="color_primary"
                     class="font-weight-bold"
                     text>
                {{ news.title }}
              </v-btn>
            </div>

            <v-card-text>

              <div class="mb-2 text-subtitle-1">
                <div class="latest-news-date pt-4"><span class="gray--text pr-2">{{ news.time }}</span>{{ news.date }}
                </div>
              </div>

              <div>
                {{ news.description }}
              </div>
            </v-card-text>
          </v-card>
        </div>

      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: "news-archive",
  layout: 'user',
  data() {
    return {
      news1: [
        {
          title: "مسابقه سازه های ماکارونی",
          time: "10:30",
          date: "08/06/1401",
          img: "construction.png",
          description: "دهمین جشواره ی سازه های ماکارونی پایه یازدهم"
        },
        {
          title: "روند پیش ثبت نام آنلاین مدرسه آینده",
          time: "10:00",
          date: "08/06/1401",
          img: "signIn.png",
          description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
        {
          title: "آزمون پذیرش میان دوره پایه دوازدهم",
          time: "09:30",
          date: "05/06/1401",
          img: "test.png",
          description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
        {
          title: "دریافت مشاوره تحصیلی",
          time: "09:30",
          date: "05/06/1401",
          img: "adviser.png",
          description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
        {
          title: "دیدار مدیر منطقه سه با جمعی از همکاران اداری",
          time: "09:00",
          date: "05/06/1401",
          img: "bos.png",
          description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
        {
          title: "جلسه انجمن اولیا مربیان",
          time: "08:30",
          date: "05/06/1401",
          img: "teacher.png",
          description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
      ],
      news2: [
        {
          title: "جمع بندی کوتاه از کارکردهای دفتر مشاوره و روانشناسی",
          time: "08:30",
          date: "05/06/1401",
          img: "office.png"
          , description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
        {
          title: "معرفی کتاب شماره 12",
          time: "08:00",
          date: "04/06/1401",
          img: "book.png",
          description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
        {
          title: "افتخار آفريني دانش‌آموزان پایه یازدهم در جشنواره همتا",
          time: "07:30",
          date: "04/06/1401",
          img: "Gifts.png"
          , description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
        {
          title: "نتايج انتخابات شوراي دانش آموزي آموزشگاه ",
          time: "07:30",
          date: "03/06/1401",
          img: "result.png",
          description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
        {
          title: "تمدید مجدد مهلت ثبت نام در آزمون های ورودی ...",
          time: "06:30",
          date: "02/06/1401",
          img: "extension.png"
          , description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },
        {
          title: "اسامی دانش آموزان حائز رتبه برتر کنکور 1401",
          time: "06:30",
          date: "01/06/1401",
          img: "Well_done.png",
          description: "متن ساختگی به عنوان توضیحات اضافه خبر متن ساختگی به عنوان توضیحات اضافه خبر"
        },

      ]
    }
  }
}
</script>


<style scoped>
.news {
  background-image: linear-gradient(rgba(255, 255, 255, .7), rgba(255, 255, 255, .7)), url("assets/Images/NewsArchive/onAir.jpg");
  min-height: 250px;
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 20px;
  font-size: 25px;
}
</style>

