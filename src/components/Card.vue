<template>
  <button
    class="
      border border-white border-opacity-100
      rounded
      pt-10
      pb-20
      hover:bg-secondary
      hover:text-textsecondary
      text-white
      font-bold
      transform transition duration-500 hover:scale-110
    "
  >
    <div class="h-1/4 flex items-stretch flex-col px-6">
      <div>
        <div class="grid grid-cols-4 grid-col-flow h-full">
          <div class="text-left"><i class="fa-solid fa-s"></i></div>
          <div></div>
          <div class="col-span-2 text-right font-light">{{ stat.date }}</div>
        </div>
      </div>
      <div class="flex">
        <h1 class="text-3xl text-left font-extrabold py-12">
          {{ stat.title }}
        </h1>
      </div>
      <div class="flex mb-4">
        <div class="flex flex-col">
        <ul>
          <div
            v-for="quality in stat.qualities"
            :key="quality"
          >
            <li class="list-disc ml-4 font-light text-left leading-normal mb-1">
            {{ quality }}
            </li>
          </div>
        </ul>
      </div>
      </div>
      <div class="flex">
        <p class="text-xl font-bold text-left py-2">
          <u class="underline">Read more</u>
        </p>
      </div>
    </div>
  </button>
</template>

<script>
export default {
  name: "Card",
  props: ["stat"],
};
</script>
