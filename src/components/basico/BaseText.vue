<script setup lang="ts">
import { inject } from 'vue';
import { KEY_SALUDO } from './keyProvider.ts';

const saludo = inject<string>(KEY_SALUDO);
</script>

<template>
  <p>{{ saludo }}</p>
</template>

<style scoped>
p {
  border: 1px blue solid;
}
</style>
