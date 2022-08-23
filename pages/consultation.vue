<template>
  <div class="mt-16">
    <div class="mt-16">
      <br>
      <div class="consultation-card ma-md-8 mx-2 font-weight-black d-flex align-center justify-center">
        دفتر مشاوره و روانشناسی
      </div>

      <div class=" ma-md-8 px-4">
        مجتمع آموزشی آینده در کنار ارائه گسترده و مؤثر خدمات آموزشی، پرورشی، پژوهشی، ورزشی، مشاوره های تحصیلی و ...،
        برای
        رشد و سلامت والاتر ذهنی و روانی دانش آموزان و خانواده های گرامی آنها، اقدام به راه اندازی دفتر روانشناسی و
        مشاوره نموده است تا به این ترتیب زمینه های بیشتر و بهتر شکوفایی و بارور شدن توانمندی های نهفته دانش آموزان در
        مسیر کسب موفقیت و احساس رضایت آنان را فراهم نماید.
      </div>

      <div class=" ma-md-8 px-4">
        <div class="pb-2 font-weight-bold text-decoration-underline color_primary--text">
          اهداف دفتر روانشناسی و مشاوره
        </div>
        هدف اصلی از ارائه مشاوره و خدمات روانشناختی ، کمک به فرد برای شناخت مشکلات و راه حل آنها و تسهیل رشد شخصی و
        روانی فرد به سمت یک بلوغ اجتماعی و تعالی بخشیدن آن است . به طور کلی اهداف این دفتر عبارت اند از:

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>کمک به تغییر رفتار مراجع</div>
        </div>

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>کمک به حل مشکلات موقعیتی</div>
        </div>

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>کمک به حل مشکلات موقعیتی</div>
        </div>

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>تأمین سلامت مثبت روانی</div>
        </div>

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>کمک به تصمیم گیری</div>
        </div>

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>توسعه روابط متقابل و انسانی با دیگران</div>
        </div>

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>توانمند سازی فرد در مقابله با آسیب های روانی و اجتماعی</div>
        </div>

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>آموزش مهارت هایی نظیر مهارت خودآگاهی ، مهارت حل مسئله ، مهارت مدیریت استرس و...</div>
        </div>

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>ارتقاء توانمندی های ذهنی و روانی فرد</div>
        </div>

        <div class="pt-2 d-flex align-center">
          <v-icon class="pl-1" color="color_primary">mdi-check</v-icon>
          <div>تقویت تفکر و نگرش سازنده و مثبت به عنوان زیر بنای تعالی و رشد</div>
        </div>

      </div>

      <div class=" ma-md-8 px-4">
        <div class="pb-2 font-weight-bold text-decoration-underline color_primary--text">
          زمان و ساعات پذیرش مراجعان
        </div>

        <div class="pa-4 mb-2 rounded-lg color_light_primary">

          <div class="d-flex">
            <div class="color_primary--text font-weight-bold">زمان مراجعه(با وقت قبلی):</div>
            <div class="pr-1">روزهای شنبه تا دوشنبه از ساعت 8:30 الی 14:30</div>
          </div>

          <div class="pt-4 d-flex">
            <div class="color_primary--text font-weight-bold">تلفن تماس جهت نوبت گیری:</div>
            <div class="pr-1">0818123456 (داخلی 181)</div>
          </div>

          <div class="pt-4 d-flex">
            <div class="color_primary--text font-weight-bold">تلفن همراه:</div>
            <div class="pr-1">09123456789</div>
          </div>

        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: "consultation",
  layout: 'user'
}
</script>

<style scoped>
.consultation-card {
  background-image: linear-gradient(rgba(255, 255, 255, .7), rgba(255, 255, 255, .7)), url("assets/Images/Consultation/advice2.jpg");
  min-height: 250px;
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 20px;
  font-size: 25px;
}
</style>
