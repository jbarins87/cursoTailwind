<template>
  <div class="container mx-auto max-w-full">
    <div class="p-2 mb-2 text-center justify bg-gradient-to-b from-indigo-500 to-blue-500 shadow-md">
      <h1 class="text-2xl md:text-3xl lg:text-4xl font-bold animate-bounce-slow">
        Hello world!
      </h1>
    </div>
    <div class="flex space-x-2 pb-2 justify-center">
      <div
        class="bg-blue-700 hover:bg-blue-900 text-white font-bold h-20 w-20 p-2 rounded-lg text-center content-center shadow-lg">
        <a href="https://vite.dev" target="_blank">
          <img src="/vite.svg" class="pb-1 m-auto" alt="Vite logo" />
          <p>Vite</p>
        </a>
      </div>
      <div
        class="bg-blue-700 hover:bg-blue-900 text-white font-bold h-20 w-20 p-2 rounded-lg text-center content-center shadow-lg">
        <a href="https://vuejs.org/" target="_blank">
          <img src="./assets/vue.svg" class="pb-1 m-auto" alt="Vue logo" />
          <p>Vue 3</p>
        </a>
      </div>
    </div>
  </div>
  <!--Container Border-box Box-content-->
  <div class="container bg-purple-300 m-4">Container 1</div>
  <div class="container bg-indigo-400 m-4 border-4 border-purple-500 border-box p-10">Container 2</div>
  <div class="container bg-pink-200 m-4 border-4 border-pink-800 box-content p-10">Container 3</div>
  <!--Container Box-->

  <!--Display Box-->
  <div class="container space-y-1 text-center m-auto">
    <span class="block w-48 m-auto bg-red-300 p-1 rounded-md">Block</span>
    <div class="inline-block mr-1 w-24 bg-blue-500 p-1 rounded-md">Inline Block</div>
    <div class="inline-block w-24 bg-blue-500 p-1 rounded-md">Inline Block</div>
    <span class="block w-48 m-auto bg-red-300 p-1 rounded-md">Block</span>
  </div>
  <!--Display Box-->

  <!--Floats e Clear-->
  <div class="container m-auto mt-2 text-center bg-red-200 p-2">
    <div class="inline-block float-start bg-red-300 p-2 m-1 shadow-lg">Exercício 1 - Float Start</div>
    <div class="inline-block float-none bg-purple-200 p-2 m-1 shadow-lg">Exercício 2 - Float None</div>
    <div class="inline-block float-end bg-green-200 p-2 m-1 shadow-lg">Exercício 3 - Float End</div>
  </div>
  <!--Floats e Clear-->

  <!--Overflow-->
  <div class="overflow-hidden h-16 m-6 bg-red-300">
    <p>Testando overflow hidden</p>
    <p>Testando overflow hidden</p>
    <p>Testando overflow hidden</p>
    <p>Testando overflow hidden</p>
    <p>Testando overflow hidden</p>
    <p>Testando overflow hidden</p>
  </div>

  <div class="overflow-auto h-16 m-6 bg-red-300">
    <p>Testando overflow auto</p>
    <p>Testando overflow auto</p>
    <p>Testando overflow auto</p>
    <p>Testando overflow auto</p>
    <p>Testando overflow auto</p>
    <p>Testando overflow auto</p>
  </div>

  <div class="overflow-x-auto h-16 m-6 bg-red-300">
    <p>
      testandooverflowxautotestandooverflowxautotestandooverflowxautotestandooverflowxautotestandooverflowxautotestandooverflowxautotestandooverflowxautotestandooverflowxautotestandooverflowxautotestandooverflowxautotestandooverflowxauto
    </p>
  </div>

  <div class="overflow-y-auto h-16 m-6 bg-red-300">
    <p>Testando overflow y-auto</p>
    <p>Testando overflow y-auto </p>
    <p>Testando overflow y-auto </p>
    <p>Testando overflow y-auto </p>
    <p>Testando overflow y-auto </p>
    <p>Testando overflow y-auto </p>
  </div>
  <!--Overflow-->

  <!--Positions-->
  <div class="relative bg-pink-300 h-20 p-2 uppercase font-bold">
    posição relative
    <div class="text-xs absolute bottom-0 right-0 bg-pink-900 text-white p-2">
      Posição Absolute - Bottom-0 Right-0
    </div>
  </div>
  <div class="container relative m-2 h-20 bg-green-100">
    <p class="p-2">Container</p>
    <div class="absolute bottom-0 right-0 bg-blue-400 p-2 text-black">
      Exercício
    </div>
  </div>
  <!--Positions-->

  <!--Visibility Hidden e Invisible-->
  <div class="container bg-teal-200">
    <button class="p-1 uppercase font-semibold bg-teal-400 h-10 w-max text-white content-center hover:bg-teal-700"
      @click.prevent="oculta()">Ocultar</button>
    <p class="inline-flex ml-2" v-show="texto">Texto de teste..</p>
  </div>

  <p class="m-2 font-medium uppercase hidden">Espaço</p>
  <p class="m-2 font-medium uppercase invisible">Espaço</p>
  <p class="m-2 font-medium uppercase visible">Espaço</p>
  <!--Visibility-->

  <!--Z Index-->
  <div class="container relative bg-orange-100 mb-48 mt-4 text-sm text-right">
    <div class="bg-orange-300 h-12 w-20 p-2 absolute z-20 shadow-md rounded-lg">Na frente</div>
    <div class="bg-orange-400 h-12 w-20 p-2 absolute z-10 m-10 shadow-md rounded-lg">No meio</div>
    <div class="bg-orange-500 h-12 w-20 p-2 absolute m-20 shadow-md rounded-lg">Atrás</div>
  </div>
  <!--Z Index-->

  <!--Flex Col e Row-->
  <div class="flex flex-row bg-red-300">
    <div class="bg-red-600 p-6 mt-2 mb-2 ml-2 uppercase font-bold">Flex Row</div>
    <div class="bg-red-600 p-6 m-2">1</div>
    <div class="bg-red-600 p-6 mt-2 mb-2">2</div>
    <div class="bg-red-600 p-6 m-2">3</div>
  </div>
  <div class="flex flex-row-reverse bg-green-300">
    <div class="bg-green-600 p-6 mt-2 mb-2 mr-2 uppercase font-bold">Flex Row Reverse</div>
    <div class="bg-green-600 p-6 m-2">1</div>
    <div class="bg-green-600 p-6 mt-2 mb-2">2</div>
    <div class="bg-green-600 p-6 m-2">3</div>
  </div>
  <div class="flex flex-col bg-blue-400 space-y-2 p-2">
    <div class="bg-red-600 p-6 uppercase font-bold">Flex Col</div>
    <div class="bg-red-600 p-6">1</div>
    <div class="bg-red-600 p-6">2</div>
    <div class="bg-red-600 p-6">3</div>
  </div>
  <div class="inline-flex space-x-2">
    <div
      class="container flex flex-col bg-gradient-to-t from-purple-100 to-purple-900 mt-10 space-y-2 text-center p-2 w-max rounded-lg">
      <div class="bg-pink-200 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-300 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-400 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-500 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-600 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-700 p-2 rounded-md">Exercícios</div>
    </div>
    <div
      class="container flex flex-col bg-gradient-to-t from-pink-100 to-pink-900 mt-10 space-y-2 text-center p-2 w-max rounded-lg">
      <div class="bg-pink-200 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-300 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-400 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-500 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-600 p-2 rounded-md">Exercícios</div>
      <div class="bg-pink-700 p-2 rounded-md">Exercícios</div>
    </div>
  </div>
  <!--Flex Col e Row-->

  <!--Flew Wrap-->
  <div class="bg-red-100 flex flex-wrap mt-2 p-1 justify-center">
    <div class="bg-pink-300 p-2 rounded-md m-2">Exercícios</div>
    <div class="bg-pink-400 p-2 rounded-md m-2">Exercícios</div>
    <div class="bg-pink-500 p-2 rounded-md m-2">Exercícios</div>
    <div class="bg-pink-600 p-2 rounded-md m-2">Exercícios</div>
    <div class="bg-pink-700 p-2 rounded-md m-2">Exercícios</div>
  </div>
  <!--Flew Wrap-->

  <!--Flex container stratch-->
  <div class="flex container bg-green-400 p-4 mt-4 text-center m-auto uppercase font-medium">
    <div class="bg-green-300 flex-1">Flex-1</div>
    <div class="bg-green-200 flex-1">Flex-1</div>
    <div class="bg-green-100 flex-none">Flex-none</div>
  </div>
  <!--Flex container-->



  <HelloWorld msg="Vite + Vue" />
</template>

<script setup>
  import { ref } from 'vue'
  import HelloWorld from './components/HelloWorld.vue'

  const texto = ref(true);

  function oculta() {
    texto.value = !texto.value
  }
</script>

<style>
  body {
    background-color: #bfdbfe;
  }
</style>