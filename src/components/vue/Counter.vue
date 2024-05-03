<script setup>
import  { ref } from "vue"

let counter = ref(5)

function add() {
  counter.value++
  console.log(counter)
}
</script>

<template>
  <div @click="add" class="text-white select-none hover:cursor-pointer bg-blue-500 rounded py-1 px-2 max-w-40 text-center">
    Numero de clics: {{ counter }}
  </div>
</template>