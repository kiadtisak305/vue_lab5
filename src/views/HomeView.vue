<script setup>
import Detail from '../components/Detail.vue';
</script>

<template>
  <main>
    <div v-for="i in 3">
      <Detail />
    </div>
  </main>
</template>
