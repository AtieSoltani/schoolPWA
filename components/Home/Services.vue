<template>
  <div class="service-card ma-8 pt-5 px-3
   d-sm-flex justify-space-around">

    <div class="d-flex flex-column align-center">
      <nuxt-link to="">
        <img src="@/assets/Images/Home/Services/kadr.png">
      </nuxt-link>
      <p class="service-card-text font-weight-bold">معرفی کادر</p>
    </div>

    <div class="d-flex flex-column align-center">
      <nuxt-link to="">
        <img src="@/assets/Images/Home/Services/moshavere.png">
      </nuxt-link>
      <p class="service-card-text font-weight-bold">واحد مشاوره و بهداشت</p>
    </div>

    <div class="d-flex flex-column align-center">
      <nuxt-link to="">
        <img src="@/assets/Images/Home/Services/eftekhar.png">
      </nuxt-link>
      <p class="service-card-text font-weight-bold">افتخارات مدرسه</p>
    </div>

  </div>
</template>

<script>
export default {
  name: "Services"
}
</script>

<style lang="scss" scoped>
.service-card{
  background-image: url("assets/Images/Home/Services/back.png");
  min-height: 250px;
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 20px;

  &-text{
    font-size: 16px;
    color: white;
  }
}

</style>
