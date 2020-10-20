<template>
  <div class="info md:mb-2 w-4/6 ">

    <p class="md:text-xl leading-none">FORM</p>
    <span class="md:text-6xl leading-none font-bold">FORM</span>
    <p class="md:text-xl mt-10">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos ab, deserunt a ex labore nisi, reprehenderit sed voluptate consectetur ipsum pariatur possimus commodi placeat dolore! Facilis ad distinctio beatae laudantium?</p>

    <button class="md:btn btn-yellow mt-8 p-4 self-center">
      Quero uma consultoria
    </button>

    
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
