<!-- 主要有三個結構1.script 2. template 3.style -->
<!-- script = vue -->
<!-- template = html片段 -->
<!-- style = css -->
<script setup>
//setp =>不用****return****
import { ref } from 'vue'
const num = ref(1)
console.log('num:', num.value)

// setInterval(() => {
//   num.value++
// }, 500)
function clickMe() {
  num.value++
}
</script>

<template>
  <div>
    {{ num }}
    <button type="button" v-on:click="clickMe">按我</button>
  </div>
</template>

<style scoped></style>
