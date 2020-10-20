<template>
  <div class="form md:mt-64 md:w-full w-2/3 place-self-center sm:place-self-center md:place-self-auto">
    <span class="md:text-2xl leading-none font-bold text-orange-500"
      >Pronto para planejar seu sossego?
    </span>
    <p class="md:text-xl leading-none my-6">
      Agende uma consultoria sem compromisso pelo formulário abaixo!
    </p>
    <form>
      <div class="mb-2">
        <label class="block font-bold" for="name">Nome: </label>
        <input
          class="shadow appearance-none border w-full py-2 px-3 text-green-800 leading-tight focus:outline-none focus:shadow-outline"
          id="name"
          type="text"
        />
      </div>
      <div class="mb-2">
        <label class="block font-bold" for="mail">E-mail: </label>
        <input
          class="shadow appearance-none border w-full py-2 px-3 text-green-800 leading-tight focus:outline-none focus:shadow-outline"
          id="mail"
          type="mail"
        />
      </div>
      <label class="block font-bold" for="profession">Estado Civil: </label>
      <div class="relative mb-2">
        <select
          class="shadow appearance-none border w-full py-2 px-3 text-green-800 leading-tight focus:outline-none focus:shadow-outline"
          id="grid-state"
        >
          <option>Solteiro(a)</option>
          <option>Casado(a)</option>
          <option>Viúvo(a)</option>
        </select>
        <div
          class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700"
        >
          <svg
            class="fill-current h-4 w-4"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 20 20"
          >
            <path
              d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
            />
          </svg>
        </div>
      </div>
      <div class="mb-2">
        <label class="block font-bold" for="profession">Profissão: </label>
        <input
          class="shadow appearance-none border w-full py-2 px-3 text-green-800 leading-tight focus:outline-none focus:shadow-outline"
          id="profession"
          type="text"
        />
      </div>
      <div class="mb-2">
        <label class="block font-bold" for="phone">Telefone/Whatsapp: </label>
        <input
          class="shadow appearance-none border w-full py-2 px-3 text-green-800 leading-tight focus:outline-none focus:shadow-outline"
          id="phone"
          type="text"
        />
      </div>
      <div class="mb-2">
        <label class="block font-bold" for="income">Renda Mensal: </label>
        <input
          class="shadow appearance-none border w-full py-2 px-3 text-green-800 leading-tight focus:outline-none focus:shadow-outline"
          id="income"
          type="number"
        />
      </div>
      <div class="text-center">
        <button class="btn btn-yellow p-4 mt-2">Enviar</button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: "Form",
  props: {
    // msg: String,
  },
};
</script>

<style scoped>
.form {
  @apply bg-blue-900 text-white p-8;
}
.btn {
  @apply font-bold py-2 px-8 rounded-full;
}
.btn-yellow {
  @apply bg-orange-500 text-white;
}
.btn-yellow:hover {
  @apply bg-orange-700;
}
</style>
