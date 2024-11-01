<script setup>
  import { ref } from 'vue'

  defineProps({
    msg: String,
  })

  const count = ref(0)
</script>

<template>
  <div class="grid grid-cols-4 gap-2 m-2">
    <div class="col-span-4 text-center">
      <h1 class="text-center text-2xl font-bold">{{ msg }}</h1>
    </div>

    <div class="m-10 col-span-4 text-center">
      <button class="bg-blue-500 px-2 py-1 rounded-lg text-white hover:bg-blue-800 shadow-md uppercase" type="button"
        @click="count++">count is {{ count }}</button>
    </div>

    <div class="card card:hover">
      <p>
        Edit
        <code class="font-semibold">components/HelloWorld.vue</code> to test HMR
      </p>
    </div>

    <div class="card card:hover">
      <p>
        Check out
        <a class="link" href="https://vuejs.org/guide/quick-start.html#local"
          target="_blank">create-vue</a>, the official Vue + Vite starter
      </p>
    </div>

    <div class="card card:hover">
      <p>
        Learn more about IDE Support for Vue in the
        <a class="link" href="https://vuejs.org/guide/scaling-up/tooling.html#ide-support"
          target="_blank">Vue Docs Scaling up Guide</a>.
      </p>
    </div>

    <div class="card card:hover">
      <p>Click on the Vite and Vue logos to learn more.</p>
    </div>

  </div>
</template>