<template>
  <div class="item">
    <vue-horizontal-list :items="items" :options="options">
      <template v-slot:default="{ item }">
          <h3>{{ item.title }}</h3>
          <div class="image-container">
            <img :src="item.image" />
          </div>
          <p>{{ item.content }}</p>
          <a class="horizontal" href=""><i>>Lire plus</i></a>
      </template>
    </vue-horizontal-list>
  </div>
</template>

<script>
import VueHorizontalList from "@/vue-horizontal-list.vue";

import Image1 from '@/assets/img/partenariat.png'
import Image2 from '@/assets/img/portrait.png'
import Image3 from '@/assets/img/ecole.png'

export default {
  name: "image-three",
  components: {
    VueHorizontalList,
  },
  data() {
    return {
      items: [
        {
          title: "Partenariat",
          content:
            "Schneider Electric s’engage dans la campagne de mécénat d’ Arts et Métiers",
          image: Image1,
        },
        {
          title: "école",
          content:
            "Qualité et responsabilité Sociale des entreprises.",
          image: Image2,
        },
        {
          title: "Portrait",
          content:
            "Ma vie d’étudiante à Arts et Métiers : Julie, en Bachelor de technologie à Bordeaux.",
          image: Image3,
        },
        {
          title: "Partenariat",
          content:
            "Schneider Electric s’engage dans la campagne de mécénat d’ Arts et Métiers",
          image: Image1,
        },
        {
          title: "école",
          content:
            "Qualité et responsabilité Sociale des entreprises.",
          image: Image2,
        },
      ],
      options: {
        responsive: [
          { end: 576, size: 1 },
          { start: 576, end: 768, size: 2 },
          { size: 3 },
        ],
      },
    };
  },
};
</script>

<style scoped>
p {
  margin-top: 4px;
  overflow: hidden;
  display: -webkit-box;
  text-overflow: ellipsis;
  word-break: break-word;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 2;
  font-size:18px;
}
.item {
  padding: 6px 24px 18px;
}
.subtitle {
  margin-top: 12px;
  font-size: 14px;
  font-weight: 500;
  margin-bottom: 6px;
}
h3 {
    display: table-cell;
}
.image-container {
  display: table-cell;
}

img {
  width: 25px;
  height: 25px;
  margin: 0 10px;
}

</style>
