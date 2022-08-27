<template>
  <div class="mt-16">
    <div class="mt-16">
      <p class="font-weight-bold px-4 pt-4 color_primary--text text-decoration-underline">فرم ثبت نام آنلاین</p>

      <v-form
        class="pa-4 d-sm-flex"
        ref="form"
        v-model="valid"
        lazy-validation
      >
        <div class="flex-grow-1 px-2">

          <v-text-field
            outlined
            class="align-center"
            v-model="name"
            :counter="12"
            :rules="nameRules"
            label="نام"
            required
            reverse
          ></v-text-field>

          <v-text-field
            outlined
            v-model="lastName"
            :counter="12"
            :rules="nameRules"
            label="نام خانوادگی"
            required
            reverse
          ></v-text-field>

          <v-text-field
            outlined
            v-model="fatherName"
            :counter="12"
            :rules="fatherNameRules"
            label="نام پدر"
            required
            reverse
          ></v-text-field>

          <v-text-field
            outlined
            v-model="id"
            :counter="10"
            :rules="idRules"
            label="شماره شناسنامه"
            required
            reverse
          ></v-text-field>

          <v-text-field
            outlined
            v-model="phone"
            :counter="8"
            :rules="phoneRules"
            label="شماره تلفن ثابت"
            required
            reverse
          ></v-text-field>

          <v-text-field
            outlined
            v-model="mobile"
            :counter="8"
            :rules="mobileRules"
            label="شماره تلفن همراه"
            required
            reverse
          ></v-text-field>


        </div>

        <div class="flex-grow-1 px-2">

          <v-text-field
            outlined
            v-model="city"
            label="شهر"
            required
            reverse
          ></v-text-field>

          <v-text-field
            outlined
            class="align-center"
            v-model="grade"
            label="مقطع تحصیلی"
            required
            reverse
          ></v-text-field>

          <v-text-field
            outlined
            v-model="major"
            label="رشته تحصیلی"
            required
            reverse
          ></v-text-field>

          <v-text-field
            outlined
            v-model="GPA"
            label="معدل"
            required
            reverse
          ></v-text-field>

          <v-textarea
            height="140"
            outlined
            label="آدرس"
            value=""
            reverse
          ></v-textarea>

        </div>

      </v-form>

   <div class="mb-4 text-left ml-8">
     <v-btn
       :disabled="!valid"
       color="color_primary white--text"
       class="mr-4"
       @click="validate"
     >
       ذخیره اطلاعات
     </v-btn>

     <v-btn
       outlined
       color="color_primary"
       class="mr-4"
       @click="reset"
     >
       باز نشانی فرم
     </v-btn>

   </div>
    </div>
  </div>

</template>

<script>

export default {
  name: "registration",
  layout: 'user',
  data: () => ({
    valid: true,
    name: '',
    nameRules: [
      v => !!v || 'وارد کردن نام و نام خانوادگی الزامی است',
      v => (v && v.length <= 12) || 'نام و نام خانوادگی باید حداکثر 12 حرف باشد - ',
    ],
    lastName: '',
    lastNameRules: [
      v => !!v || 'وارد کردن نام و نام خانوادگی الزامی است',
      v => (v && v.length <= 12) || 'نام و نام خانوادگی باید حداکثر 12 حرف باشد - ',
    ],
    fatherName: '',
    fatherNameRules: [
      v => !!v || 'وارد کردن نام پدر الزامی است',
      v => (v && v.length <= 12) || 'نام پدر باید حداکثر 12 حرف باشد - ',
    ],
    phone: '',
    phoneRules: [
      v => !!v || 'وارد کردن شماره تلفن ثابت الزامی است ',
      v => (v && v.length === 8) || 'اعداد شماره تلفن باید برابر با 8 باشد - ',
    ],
    mobile: '',
    mobileRules: [
      v => !!v || 'وارد کردن شماره تلفن همراه الزامی است ',
      v => (v && v.length === 11) || 'شماره تلفن همراه باید 11 رقم باشد - ',

    ],
    id:'',
    idRules:[
      v => !!v || 'وارد کردن شماره شناسنامه الزامی است ',
      v => (v && v.length === 10) || 'شماره شناسنامه باید 10 رقم باشد - ',
    ],

    city:'',
    grade:'',
    major:'',
    GPA:'',
  }),

  methods: {
    validate() {
      this.$refs.form.validate()
    },
    reset() {
      this.$refs.form.reset()
    },
  },
}
</script>

<style scoped>

</style>
