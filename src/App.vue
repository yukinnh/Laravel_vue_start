<template>
  <div id="app">
    <p>Vue3公式サイトは<a v-bind:href="link">こちら</a></p>
  </div>
</template>

<script setup>
const link = "https://v3.ja.vuejs.org/"
</script>