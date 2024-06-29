<script setup lang="ts">
import { provide, ref, type Ref, reactive } from 'vue';
import ComponenteIntermedio from './ComponenteIntermedio.vue';

const num: Ref<number> = ref(0);

const increment = () => {
  num.value++;
};

provide('num', { num, increment });
</script>
<template>
  <section>
    <ComponenteIntermedio />
  </section>
</template>

<style scoped>
section {
  border: 1px green solid;
  padding: 5px;
}
</style>
