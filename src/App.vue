<template>
  <div id="app">
    <form>
      <select id ="language" v-model= "language">
        <option value="">好きなプログラミング言語を選んでください。</option>
        <option value="php">PHP</option>
        <option value="ruby">Ruby</option>
        <option value="python">Python</option>
        <option value="java">Java</option>
      </select>
    </form>
    <div v-if="language==='php'">Web系でよく使用されている</div>
    <div v-else-if="language==='ruby'">日本発のプログラミング言語</div>
    <div v-else-if="language==='python'">機械学習で使用されることが多い</div>
    <div v-else-if="language==='java'">大規模開発で用いられることが多い言語</div>
    <div v-else>プログラミング言語が選択されていません。</div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const language = ref(null);
</script>