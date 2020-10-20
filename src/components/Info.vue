<template>
  <div
    class="info md:mt-20 sm:my-6 my-6 md:ml-8 p-6 md:p-4 sm:w-1/2 md:w-full xl:h-4/12 lg:h-1/2 md:h-2/5 h-auto place-self-center sm:place-self-center md:place-self-auto"
  >
    <p class="md:text-xl leading-none">Vida toda</p>
    <span class="text-6xl leading-none font-black break-words">BEM ESTAR</span>
    <p class="md:text-xl mt-10">Soluções completas para viver mais e melhor</p>
    <div class="text-center mt-8 xl:mt-6 md:mt-4">
      <button class="btn btn-yellow p-4 self-center">
        Quero uma consultoria
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Info",
  props: {
    // msg: String,
  },
};
</script>

<style scoped>
.info {
  @apply border-4 border-blue-900 text-blue-900 bg-white opacity-75;
}

.info:hover {
  @apply opacity-100;
}

.btn {
  @apply font-bold py-2 px-3;
}
.btn-yellow {
  @apply bg-yellow-500 text-white;
}
.btn-yellow:hover {
  @apply bg-yellow-700;
}
</style>
