<script setup lang="ts">
import { useDragAndDrop } from "@formkit/drag-and-drop/vue";
const [parent, tapes] = useDragAndDrop([
  "Depeche Mode",
  "Duran Duran",
  "Pet Shop Boys",
  "Kraftwerk",
  "Tears for Fears",
  "Spandau Ballet",
]);
</script>

<template>
  <ul ref="parent">
    <li v-for="tape in tapes" :key="tape" class="cassette">
      {{ tape }}
    </li>
  </ul>
</template>
