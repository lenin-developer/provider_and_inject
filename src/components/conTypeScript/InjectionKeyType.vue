<script setup lang="ts">
import { provide, ref, type Ref } from 'vue';
import ComponenteIntermedio from './ComponenteIntermedio.vue';
import { KEY_TEXT } from './keyProvider.ts';

const text: Ref<string> = ref('soy un texto');
provide(KEY_TEXT, text);
</script>
<template>
  <section>
    <ComponenteIntermedio />
    <span>externo</span>
    <input type="text" v-model="text" />
  </section>
</template>

<style scoped>
section {
  border: 1px green solid;
  padding: 5px;
}
</style>
