<template>
  <div id="app" class="">
    <div class="relative pb-2/3">
      <img
        class="absolute h-full w-full object-cover"
        alt="Banner"
        src="@/assets/img/banner.jpg"
      />
    </div>
    <div
      class="md:absolute md:top-0 md:mt-56 mx-6 md:mr-8 grid md:grid-cols-2 md:gap-x-40"
    >
      <Info />
      <Form />
    </div>
    <div class="md:mt-64 md:ml-2 sm:mt-6 mt-4 sm:ml-40 ml-40 md:w-2/6 sm:w-1/2 w-2/5 border border-blue-700">
      <div class="text-orange-500 text-xl font-semibold">Pense nisso...</div>
      <div class="text-blue-800 text-lg font-medium">
        O quanto o diagnóstico de uma doença grave, internação ou cirurgia
        inesperada pode afetar, hoje a suavida pessoal e financeira?
      </div>
    </div>
    <div class="pb-2/3"></div>
  </div>
</template>

<script>
import Info from "./components/Info.vue";
import Form from "./components/Form.vue";

export default {
  name: "App",
  components: {
    Info,
    Form,
  },
};
</script>
<style>
</style>
