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
  <br>
  <hr>

  <!--Display Box-->
  <div class="container space-y-1 text-center m-auto">
    <span class="block w-48 m-auto bg-red-300 p-1 rounded-md">Block</span>
    <div class="inline-block mr-1 w-24 bg-blue-500 p-1 rounded-md">Inline Block</div>
    <div class="inline-block w-24 bg-blue-500 p-1 rounded-md">Inline Block</div>
    <span class="block w-48 m-auto bg-red-300 p-1 rounded-md">Block</span>
  </div>
  <!--Display Box-->
  <br>
  <hr>

  <!--Floats e Clear-->
  <div class="container m-auto mt-2 text-center bg-red-200 p-2">
    <div class="inline-block float-start bg-red-300 p-2 m-1 shadow-lg">Exercício 1 - Float Start</div>
    <div class="inline-block float-none bg-purple-200 p-2 m-1 shadow-lg">Exercício 2 - Float None</div>
    <div class="inline-block float-end bg-green-200 p-2 m-1 shadow-lg">Exercício 3 - Float End</div>
  </div>
  <!--Floats e Clear-->
  <br>
  <hr>

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
  <br>
  <hr>

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
  <br>
  <hr>

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
  <br>
  <hr>

  <!--Z Index-->
  <div class="container relative bg-orange-100 mb-48 mt-4 text-sm text-right">
    <div class="bg-orange-300 h-12 w-20 p-2 absolute z-20 shadow-md rounded-lg">Na frente</div>
    <div class="bg-orange-400 h-12 w-20 p-2 absolute z-10 m-10 shadow-md rounded-lg">No meio</div>
    <div class="bg-orange-500 h-12 w-20 p-2 absolute m-20 shadow-md rounded-lg">Atrás</div>
  </div>
  <!--Z Index-->
  <br>
  <hr>

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
  <br>
  <hr>

  <!--Flew Wrap-->
  <div class="bg-red-100 flex flex-wrap mt-2 p-1 justify-center">
    <div class="bg-pink-200 p-2 px-3 py-1 rounded-md m-2">Flex-Wrap</div>
    <div class="bg-pink-300 p-2 px-3 py-1 rounded-md m-2">01</div>
    <div class="bg-pink-400 p-2 px-3 py-1 rounded-md m-2">02</div>
    <div class="bg-pink-500 p-2 px-3 py-1 rounded-md m-2">03</div>
    <div class="bg-pink-600 p-2 px-3 py-1 rounded-md m-2">04</div>
    <div class="bg-pink-700 p-2 px-3 py-1 rounded-md m-2">05</div>
  </div>
  <!--Flew Wrap-->
  <br>
  <hr>

  <!--Flex container stratch-->
  <div class="flex container bg-green-400 p-4 mt-4 text-center m-auto uppercase font-medium">
    <div class="bg-green-300 flex-1">Flex-1</div>
    <div class="bg-green-200 flex-1">Flex-1</div>
    <div class="bg-green-100 flex-none">Flex-none</div>
  </div>
  <!--Flex container-->
  <br>
  <hr>

  <!--Order-->
  <div class="bg-purple-100 flex flex-wrap mt-2 p-1 justify-center text-white text-center">
    <div class="bg-purple-300 px-3 py-1 w-32 rounded-md m-2 order-last"><p>01</p> (order-last)</div>
    <div class="bg-purple-400 px-3 py-1 w-32 rounded-md m-2 order-5"><p>02</p> (order-5)</div>
    <div class="bg-purple-500 px-3 py-1 w-32 rounded-md m-2 order-4"><p>03</p> (order-4)</div>
    <div class="bg-purple-600 px-3 py-1 w-32 rounded-md m-2 order-3"><p>04</p> (order-3)</div>
    <div class="bg-purple-700 px-3 py-1 w-32 rounded-md m-2 order-2"><p>05</p> (order-2)</div>
    <div class="bg-purple-800 px-3 py-1 w-32 rounded-md m-2 order-first"><p>06</p> (order-first)</div>
  </div>

  <div class="container flex flex-wrap mt-2 bg-gray-600 rounded-md justify-center m-auto shadow-lg">
    <div class="bg-gray-200 p-2 rounded-md m-2 font-bold px-3 py-1 shadow-inner lg:order-last">01</div>
    <div class="bg-gray-200 p-2 rounded-md m-2 font-bold px-3 py-1 shadow-inner lg:order-2">02</div>
    <div class="bg-gray-200 p-2 rounded-md m-2 font-bold px-3 py-1 shadow-inner lg:order-first">03</div>
  </div>
  <!--Order-->
  <br>
  <hr>
  <br>
  <!--Grid Col-->
  <p class="text-lg font-bold uppercase text-center bg-white/40">grid com 3 colunas</p>
  <div class="m-auto grid grid-cols-3 bg-white text-center gap-2 p-2">
    <div class="bg-orange-200 rounded-md shadow-md">1</div>
    <div class="bg-orange-300 rounded-md shadow-md">2</div>
    <div class="bg-orange-400 rounded-md shadow-md">3</div>
    <div class="bg-orange-500 rounded-md shadow-md">4</div>
  </div>
  <div class="grid grid-cols-2 bg-orange-500 text-center gap-2 p-2 font-semibold">
    <div class="bg-gray-400 border-2 border-white/50 rounded-md">1</div>
    <div class="bg-gray-400 border-2 border-white/50 rounded-md">2</div>
  </div>
  <br>
  <div class="container grid grid-cols-3 bg-lime-200 text-center font-bold gap-2 p-2 rounded-md m-auto">
    <div class="bg-lime-500 rounded-md shadow-md">1</div>
    <div class="bg-lime-600 rounded-md shadow-md">2</div>
    <div class="bg-lime-700 rounded-md shadow-md">3</div>
    <div class="bg-lime-500 rounded-md shadow-md">4</div>
    <div class="bg-lime-600 rounded-md shadow-md">5</div>
    <div class="bg-lime-700 rounded-md shadow-md">6</div>
    <div class="bg-lime-500 rounded-md shadow-md">7</div>
    <div class="bg-lime-600 rounded-md shadow-md">8</div>
    <div class="bg-lime-700 rounded-md shadow-md">9</div>
  </div>
  <!--Grid Col-->
  <br>
  <hr>
  <br>




  <!-- <HelloWorld msg="Vite + Vue" /> -->
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