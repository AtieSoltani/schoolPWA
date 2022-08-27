<template>
  <div class="latest-news ma-md-8 ma-2 rounded-lg overflow-x-hidden">

    <p class="latest-news-title px-4 text-decoration-underline">آخرین اخبار</p>

    <div class="pa-4 d-md-flex color_light_primary rounded-xl justify-space-around">

      <div>
        <div v-for="(news , i) in news1" :key="i" class="py-2 d-flex align-center overflow-x-hidden">

            <v-img :src="require(`@/assets/Images/Home/LatestNews/${news.img}`)"
                   max-width="50"
                   height="50"
                   class="latest-news-img rounded-circle"></v-img>
            <v-btn nuxt to=""
                   color="color_primary"
                   class="font-weight-bold"
            text>
              {{news.title}}
            </v-btn>
            <p class="latest-news-date pt-4">{{news.date}}</p>

        </div>
      </div>

      <div>
        <div v-for="(news , i) in news2" :key="i" class="py-2 d-flex align-center overflow-x-hidden">

          <v-img :src="require(`@/assets/Images/Home/LatestNews/${news.img}`)"
                 max-width="50"
                 height="50"
                 class="latest-news-img rounded-circle"></v-img>
          <v-btn nuxt to=""
                 color="color_primary"
                 class="font-weight-bold"
                 text>
            {{news.title}}
          </v-btn>
          <p class="pt-3">{{news.date}}</p>

        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: "LatestNews",
  data() {
    return {
      news1: [
        {title: "مسابقه سازه های ماکارونی", time:"10:30",date: "08/06/1401", img: "construction.png"},
        {title: "روند پیش ثبت نام آنلاین مدرسه آینده", time:"10:00", date: "08/06/1401", img: "signIn.png"},
        {title: "آزمون پذیرش میان دوره پایه دوازدهم", time:"09:30", date: "05/06/1401", img: "test.png"},
        {title: "دریافت مشاوره تحصیلی", time:"09:30", date: "05/06/1401", img: "adviser.png"},
        {title: "دیدار مدیر منطقه سه با جمعی از همکاران اداری", time:"09:00", date: "05/06/1401", img: "bos.png"},
        {title: "جلسه انجمن اولیا مربیان", time:"08:30", date: "05/06/1401", img: "teacher.png"},
      ],
      news2: [
        {title: "جمع بندی کوتاه از کارکردهای دفتر مشاوره و روانشناسی", time:"08:30", date: "05/06/1401", img: "office.png"},
        {title: "معرفی کتاب شماره 12", time:"08:00", date: "04/06/1401", img: "book.png"},
        {title: "افتخار آفريني دانش‌آموزان پایه یازدهم در جشنواره همتا", time:"07:30", date: "04/06/1401", img: "Gifts.png"},
        {title: "نتايج انتخابات شوراي دانش آموزي آموزشگاه ", time:"07:30", date: "03/06/1401", img: "result.png"},
        {title: "تمدید مجدد مهلت ثبت نام در آزمون های ورودی مدارس سمپاد", time:"06:30", date: "02/06/1401", img: "extension.png"},
        {title: "اسامی دانش آموزان حائز رتبه برتر کنکور 1401" , time:"06:30", date: "01/06/1401", img: "Well_done.png"},

      ]
    }
  },

}
</script>

<style lang="scss" scoped>
.latest-news {
  &-title {
    color: $color-primary;
    font-size: 18px;
    font-weight: bold;
  }

  &-box {
    border-radius: 30px;
  }

  &-date{
font-size: 12px;
  }
}
</style>
