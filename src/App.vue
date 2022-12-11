<template>
  <form>
    <div for="name">名前を入力してください</div>
    <input type="text" id="name" v-model= "myLastName" />
  </form>
  <div>私の名前は、{{ myLastName }} です。</div>
</template>

<script setup>
import { ref } from "vue";
const myLastName = ref(null);
</script>