<script setup lang="ts">
import { provide, ref, type Ref } from 'vue';
import ComponenteIntermedio from './ComponenteIntermedio.vue';
import { KEY_SALUDO } from './keyProvider.ts';

const saludo: Ref<string> = ref('hola vue');
provide(KEY_SALUDO, saludo);
</script>
<template>
  <section>
    <ComponenteIntermedio />
    <span>externo</span>
    <input type="text" v-model="saludo" />
  </section>
</template>

<style scoped>
section {
  border: 1px green solid;
  padding: 5px;
}
</style>
