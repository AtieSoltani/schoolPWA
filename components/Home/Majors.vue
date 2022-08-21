<template>
  <div class="majors pa-4 mx-8 d-md-flex justify-space-between">

    <div class="d-none d-md-flex d-lg-flex">
      <img class="majors-img" src="@/assets/Images/Home/education.png">
    </div>

    <div>

      <p class="majors-title text-decoration-underline">رشته های تحصیلی</p>

      <div>

        <div class="py-2">
          <div class=" pb-1 font-weight-bold">
            <v-icon color="color_primary" class="pl-1">mdi-account-school</v-icon>
            ریاضی فیزیک
          </div>
          <div class="pr-4">
            نام رشته ریاضی فیزیک، با رشته‌های فنی و مهندسی دانشگاه‌ها عجین شده‌است؛ بنابراین اکثر مشاغل فنی و مهندسی،
            از طریق تحصیل در رشته ریاضی و فیزیک قابل دسترسی خواهد بود.
          </div>
        </div>

        <div class="py-2">
          <div class=" pb-1 font-weight-bold">
            <v-icon color="color_primary" class="pl-1">mdi-account-school</v-icon>
            علوم تجربی
          </div>
          <div class="pr-4">
            رشته علوم تجربی از رشته‌های شاخه نظری و یکی از رشته‌های پرطرفدار در میان دانش‌آموزان پایه نهم است. دانش
            آموزان علاقمند به رشته‌های پزشکی در این رشته تحصیل می کنند.
          </div>
        </div>

        <div class="py-2">
          <div class=" pb-1 font-weight-bold">
            <v-icon color="color_primary" class="pl-1">mdi-account-school</v-icon>
            علوم انسانی
          </div>
          <div class="pr-4">
            اگر شغل‌های محبوب وکالت، مدیریت و روانشناسی را دوست دارید، شما باید در سال نهم دبیرستان رشته‌ی علوم انسانی را انتخاب کنید تا بتوانید با شرکت در کنکور علوم انسانی وارد این رشته‌ها شوید.
          </div>
        </div>

      </div>

    </div>

  </div>
</template>

<script>
export default {
  name: "Majors"
}
</script>

<style scoped lang="scss">
.majors {
  &-title {
    color: $color-primary;
    font-size: 18px;
    font-weight: bold;
  }

  &-img {
    max-height: 377px;
    max-width: 489px;
  }
}

</style>
