<template>
  <main class="p-10" ref="test">
    <button @click="addPropertyToObject" class="p-4 rounded-3xl bg-gray-700 mr-2 text-white">+</button>
    <div>{{ state.a }}</div>
    <button @click="updateString" class="p-4 rounded-3xl bg-gray-700 text-white">-</button>
  </main>
</template>


<script setup>

import {onMounted, ref} from "vue";

let state = ref({ a: 10 })


const test = ref(null)

const addPropertyToObject = () => {
  state.value = { a: 100 }
}

const updateString = () => {
  state.value.b = 30
}


onMounted(() => {
  console.log(test.value)
})



</script>


