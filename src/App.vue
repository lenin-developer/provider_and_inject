<script setup lang="ts">
import { provide, ref, type Ref } from 'vue';
import BaseProviderInject from './components/basico/BaseProviderInject.vue';
import ProviderInjectUpdateData from './components/updateData/ProviderInjectUpdateData.vue';
import InjectionKeyType from './components/conTypeScript/InjectionKeyType.vue';

const saludo: Ref<string> = ref('hola vue');
provide('saludo', saludo);
</script>
<template>
  <p>nota el valor por defeault no funciona como dice en la doc</p>
  <br />
  <h2>injecion basico</h2>
  <BaseProviderInject />

  <h2>injeccion con actualizacion</h2>
  <ProviderInjectUpdateData />

  <h2>type injectionKey</h2>
  <InjectionKeyType />
</template>

<style scoped></style>
