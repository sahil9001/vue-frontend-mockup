<template>
<div class="pt-52 pb-10">
  <div class="grid grid-cols-3 gap-4">
    <div class="col-span-2">
        <div class="flex flex-col">
            <div class="flex-1 mb-10">  <h1 class="font-extrabold leading-normal text-5xl tracking text-white">Creative Digital Design Agency is looking for new <u class="underline w-10">talent</u></h1>
    </div>
    <div class="flex-1">
  <button class="border border-white border-opacity-100 rounded px-10 py-2 hover:bg-white hover:text-primary text-white font-bold">
      Send a Resume
  </button>
    
    </div>
        </div>
    </div>
    <div>
        <img src="../assets/1.png" class=""/>
    </div>
  </div>
</div>
<Cards />
</template>

<script>
import Cards from '../components/Cards.vue'
export default {
  name: "Body",
  components: {
    Cards
  }
};
</script>
