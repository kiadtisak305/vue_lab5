<script setup>
import { RouterView } from "vue-router";
</script>

<template>
  <header>
    <section class="py-5 text-center container">
      <div class="wrapper">
        <div class="greetings">
          <h1 class="green">Album example</h1>
        </div>
      </div>
    </section>
  </header>
  
  <RouterView />
</template>

<style scoped>

header {
  line-height: 1.5;
  max-height: 100vh;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
