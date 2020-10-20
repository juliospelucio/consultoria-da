<template>
  <div id="app" class="">
    <div class="relative pb-2/3">
      <img
        class="absolute h-full w-full object-cover"
        alt="Banner"
        src="@/assets/img/banner.jpg"
      />
    </div>
      <div class="relative grid md:grid-cols-2 gap-x-64 mt-4">
        <Info msg="Welcome to Your Vue.js App" />
        <Form msg="Welcome to Your Vue.js App" />
      </div>
  </div>
</template>

<script>
import Info from "./components/Info.vue";
import Form from "./components/Form.vue";

export default {
  name: "App",
  components: {
    Info,
    Form
  },
};
</script>
<style>
</style>
