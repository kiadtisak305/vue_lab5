<script setup>
import { ref } from 'vue';
const like = ref(0);
const sad = ref(0);

function likeClick() {
    like.value += 1;
}
function SadClick() {
    sad.value -= 1;
}


</script>

<template>
    <div class="btn-group">
        <button class="btn btn-sm btn-outline-secondary" @click="likeClick()">
            <span class="material-symbols-outlined">
                favorite
            </span>
            {{ like }}
        </button>

        <button class="btn btn-sm btn-outline-secondary" @click="SadClick()">
            <span class="material-symbols-outlined">
                sentiment_dissatisfied
            </span>
            {{ sad }}
        </button>

    </div>

</template>

<style scoped>
.material-symbols-outlined {
  font-variation-settings:
  'FILL' 0,
  'wght' 400,
  'GRAD' 0,
  'opsz' 48
}
</style>