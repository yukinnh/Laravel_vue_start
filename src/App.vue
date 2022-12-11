<template>
  <div id ="app">
    <div>Vue3 基礎編</div><br>
    <button @click="onClick">現在の時間を取得します</button>
    <p>{{ time }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";
const time = ref(null);
const onClick = () => {
  time.value = new Date().toTimeString();
}

</script>

<style>
/* CSSは書かない */
</style>
