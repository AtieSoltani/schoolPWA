<template>
  <div class="mt-16">
    <div class="mt-16">
      <br>
      <gallery-card :img="img1" :title="title1"/>
      <gallery-card :img="img2" :title="title2"/>

    </div>
  </div>
</template>

<script>
import GalleryCard from "~/components/Gallery/GalleryCard";
export default {
  name: 'InspirePage',
  layout: 'user',
  components:{
    GalleryCard
  },
  data: () => ({
    title1:"اردوی فرهنگی تاریخی مسجد جامع یزد مدرسه آینده",
    img1: ["1.1.jpg", "1.2.jpg", "1.3.jpg", "1.4.jpg", "1.5.jpg", "1.6.jpg"],
    title2:"اردوی تفریحی آبشار و کتیبه های گنج نامه مدرسه آینده",
    img2: ["2.1.jpg", "2.2.jpg", "2.3.jpg", "2.4.jpg", "2.5.jpg", "2.6.jpg"],

  }),
}
</script>
