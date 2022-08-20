<template>
  <div class="mt-16">
    <div class="mt-16">
      <home-carousel/>
    </div>
    <services/>
  </div>
</template>

<script>
import HomeCarousel from "~/components/Home/HomeCarousel";
import Services from "~/components/Home/Services";

export default {
  layout: 'user',
  name: 'IndexPage',
  components: {
    HomeCarousel,
    Services
  }
}
</script>
