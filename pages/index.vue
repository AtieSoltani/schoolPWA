<template>
  <div class="mt-16">
    <div class="mt-16">
      <home-carousel/>
    </div>
    <services/>
    <facilities/>
    <majors/>
    <latest-news/>
    <basic-information/>
  </div>
</template>

<script>
import HomeCarousel from "~/components/Home/HomeCarousel";
import Services from "~/components/Home/Services";
import Facilities from "~/components/Home/Facilities";
import Majors from "~/components/Home/Majors";
import LatestNews from "~/components/Home/LatestNews";
import BasicInformation from "~/components/Home/BasicInformation";

export default {
  layout: 'user',
  name: 'IndexPage',
  components: {
    HomeCarousel,
    Services,
    Facilities,
    Majors,
    LatestNews,
    BasicInformation
  }
}
</script>
