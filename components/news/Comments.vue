<template>
  <v-form
    ref="form"
    v-model="valid"
    lazy-validation
  >
    <v-text-field
      v-model="name"
      :counter="20"
      :rules="nameRules"
      label="نام و نام خانوادگی"
      required
      reverse

    ></v-text-field>

    <v-text-field
      v-model="email"
      :rules="emailRules"
      label="ایمیل"
      required
      reverse
    ></v-text-field>

    <v-textarea
    label="دیدگاه خود را وارد کنید"
    reverse
    ></v-textarea>


<div class="d-flex justify-space-between">
  <v-checkbox
    v-model="checkbox"
    label="عمومی کردن نظر"
    required
  ></v-checkbox>

  <v-btn
    :disabled="!valid"
    color="color_primary"
    class="mr-4"
    @click="validate"
  >
    ارسال نظر
  </v-btn>
</div>

  </v-form>
</template>

<script>
export default {
  name: "Comments",
  data: () => ({
    valid: true,
    name: '',
    nameRules: [
      v => !!v || 'وارد کردن نام و نام خانوادگی الزامی است',
      v => (v && v.length <= 20) || ' نام خانوادگی باید حداکثر 20 حرف باشد -',
    ],
    email: '',
    emailRules: [
      v => !!v || 'وارد کردن ایمیل اجباری است',
      v => /.+@.+\..+/.test(v) || 'ایمیل معتبر نیست',
    ],
    checkbox: false,
  }),

  methods: {
    validate () {
      this.$refs.form.validate()
    },
  },
}
</script>

<style scoped>

</style>
