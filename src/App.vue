<template>
  <div id="app">
    <div class="relative pb-2/3">
      <img
        class="absolute h-full w-full object-cover"
        alt="Banner"
        src="@/assets/img/banner.jpg"
      />
    </div>
    <div
      class="md:absolute md:top-0 md:mt-48 mx-6 md:mr-8 grid md:grid-cols-2 md:gap-x-40"
    >
      <Info />
      <Form />
    </div>
    <div
      class="xl:mt-10 lg:mt-12 md:mt-40 sm:mt-6 mt-4 md:ml-20 sm:ml-40 ml-6 md:w-2/6 sm:w-1/2 w-10/12 text-justify leading-tight"
    >
      <div class="text-orange-500 text-xl font-semibold">Pense nisso...</div>
      <div class="text-blue-800 text-lg font-medium">
        O quanto o diagnóstico de uma doença grave, internação ou cirurgia
        inesperada pode afetar, hoje a sua vida pessoal e financeira?
      </div>
    </div>
    <div
      class="bg-blue-900 p-8 text-white text-center font-bold text-4xl mt-5 xl:mt-8 md:mt-32 xl:w-3/4 lg:w-1/2 md:w-7/12 sm:w-full"
    >
      Blog
    </div>
    <div
      class="mt-5 grid xl:grid-cols-3 xl:gap-x-4 lg:grid-cols-3 lg:gap-4 md:grid-cols-2 md:gap-x-4 sm:grid-cols-1 gap-x-4 mx-1 justify-items-center"
    >
      <div
        v-for="post in posts"
        :key="post.id"
        class="max-w-sm overflow-hidden shadow-lg border-4 border-blue-900 my-1"
      >
        <img class="w-full" src="@/assets/img/banner.jpg" alt="Floresta" />
        <div class="px-6 py-4">
          <div class="font-bold mb-2">{{ post.title }}</div>
          <p class="text-gray-700 text-base">
            {{ post.body }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Info from "./components/Info.vue";
import Form from "./components/Form.vue";
import axios from "axios";

export default {
  name: "App",
  components: {
    Info,
    Form,
  },
  data() {
    return {
      posts: null,
    };
  },
  mounted() {
    axios
      .get("https://jsonplaceholder.typicode.com/posts")
      .then((response) => (this.posts = response.data))
      .catch((error) => console.log(error));
  },
};
</script>
<style>
</style>
