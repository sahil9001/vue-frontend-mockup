<template>
  <div class="mt-10">
    <div class="flex flex-wrap items-stretch">
      <div class="w-full sm:w-1/2 md:w-1/3 lg:w-1/6 xl:w-1/4 mb-4" v-for="stat in stats"  :key="stat.id" ><Card :stat="stat"/></div>
    </div>
  </div>
</template>

<script>
import Card from './Card.vue'
export default {
  name: "Cards",
    components: {
      Card
    },
props: {
      stat : {}
  },
  data() {
    return {
      stats: [
        {
          id: "1",

          date: "03 Oct 2021",
          title: "Middle UX/UI Designer",
          qualities: ["3+ years of consumer design experience.", "Strong portfolio of completed design projects"],
        },
        {
          id: "2",
          date: "03 Oct 2021",
          title: "Senior PHP Developer",
          qualities: [],
        },
        {
          id: "3",

          date: "03 Oct 2021",
          title: "Middle Graphic Designer",
          qualities: [],
        },
        {
          id: "4",

          date: "03 Oct 2021",
          title: "Senior Ruby Developer",
          qualities: [],
        },
      ],
    };
  },
};
</script>
