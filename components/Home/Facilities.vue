<template>
  <div class="facilities pa-4 mx-8 d-md-flex justify-space-between">
    <div>

      <p class="facilities-title text-decoration-underline">تجهیزات و امکانات</p>

      <div>

        <div class="py-2">
          <v-icon color="color_primary" class="pl-1">mdi-checkbox-marked-circle-outline</v-icon>
          بهره گیری از کادر اجرایی و آموزشی مجرب و متخصص
        </div>

        <div class="py-2">
          <v-icon color="color_primary" class="pl-1">mdi-checkbox-marked-circle-outline</v-icon>
          گزینش و جذب فراگیران توانمند و نخبه از طریق آزمون ورودی
        </div>

        <div class="py-2">
          <v-icon color="color_primary" class="pl-1">mdi-checkbox-marked-circle-outline</v-icon>
          آموزش تکمیلی فراتر از کتاب مانند زبان، رایانه، المپیاد، تیزهوشان، کانگورو و ...
        </div>

        <div class="py-2">
          <v-icon color="color_primary" class="pl-1">mdi-checkbox-marked-circle-outline</v-icon>
          مجهز به آزمایشگاه‌های فیزیک، شیمی، زیست و کارگاه فناوری
        </div>

        <div class="py-2">
          <v-icon color="color_primary" class="pl-1">mdi-checkbox-marked-circle-outline</v-icon>
          دارای 3 سالن چند منظوره (امتحانات، اجتماعات، همایش ها) با گنجایش بالغ بر 200 نفر در هر سالن
        </div>

        <div class="py-2">
          <v-icon color="color_primary" class="pl-1">mdi-checkbox-marked-circle-outline</v-icon>
          سالن سرپوشیده ورزشی چند منظوره و زمین‌های ورزشی فوتبال، بسکتبال، والیبال، بدمینتون و پینگ پنگ
        </div>

      </div>

    </div>

    <div class="d-none d-md-flex d-lg-flex">
      <img class="facilities-img" src="@/assets/Images/Home/Bookshelves.png">
    </div>

  </div>
</template>

<script>
export default {
  name: "Facilities",
}
</script>

<style lang="scss" scoped>
.facilities {
  &-title {
    color: $color-primary;
    font-size: 18px;
    font-weight: bold;
  }
  &-img{
    max-height:377px ;
    max-width: 489px;
  }
}
</style>
