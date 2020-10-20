<template>
  <div class="info ml-8 my-2 sm:w-1/2 md:w-auto md:h-2/3 place-self-center sm:place-self-center md:place-self-auto">
    <p class="md:text-xl leading-none">Vida toda</p>
    <span class="md:text-6xl leading-none font-bold">BEM ESTAR</span>
    <p class="md:text-xl mt-10">Soluções completas para viver mais e melhor</p>
    <div class="text-center mt-8 md:mt-16">
      <button class="md:btn btn-yellow  p-4 self-center">
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
  @apply border-4 border-blue-700 text-blue-700 p-6;
}

.btn {
  @apply font-bold py-2 px-3;
}
.btn-yellow {
  @apply bg-yellow-500 text-white;
}
.btn-blue:hover {
  @apply bg-blue-700;
}
</style>
