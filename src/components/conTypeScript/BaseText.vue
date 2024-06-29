<script setup lang="ts">
import { inject } from 'vue';
import { KEY_TEXT } from './keyProvider.ts';

const text = inject(KEY_TEXT);
</script>

<template>
  <p>{{ text }}</p>
</template>

<style scoped>
p {
  border: 1px blue solid;
}
</style>
