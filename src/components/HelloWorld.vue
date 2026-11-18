<script setup lang="ts">
import { ref } from 'vue';

const text = ref('');


</script>

<template>
  <section>
    <input v-model="text" />
    <p v-if="text === ''">何か入力してください</p>
    <p v-else>入力中...</p>
    <p>{{ text }}</p>
  </section>
</template>
