<script setup lang="ts">
import { inject } from 'vue';
import { KEY_NUM } from './keyProvider.ts';

const { num } = inject<string>(KEY_NUM);
</script>

<template>
  <p>{{ num }}</p>
</template>

<style scoped>
p {
  border: 1px blue solid;
}
</style>
