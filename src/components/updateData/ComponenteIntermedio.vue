<script setup lang="ts">
import { inject } from 'vue';
import BaseText from './BaseText.vue';
import { KEY_NUM } from './keyProvider.ts';

const { increment } = inject(KEY_NUM);
</script>

<template>
  <div>
    <a href="https://vuejs.org/" target="_blank">
      <img src="../../assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
    <BaseText />
    <button @click="increment">increment</button>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
div {
  border: 1px red solid;
}
</style>
