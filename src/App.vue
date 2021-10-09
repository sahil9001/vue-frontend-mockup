<template>
  <NavBar />
  <div class="bg-primary">
    <div class="max-w-7xl mx-auto px-2 pb-10 sm:px-6 lg:px-8">
      <Body />
    </div>
    <Footer />
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Body from "@/components/Body.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: "App",
  components: {
    NavBar,
    Footer,
    Body,
  },
};
</script>
