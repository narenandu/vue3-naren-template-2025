<script setup lang="ts">
import { ref } from 'vue'


defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>

  <div>
    <h1 class="p-8">{{ msg }}</h1>
  </div>

  <div class="p-8">
    <button class="bg-sky-500 hover:bg-sky-700 text-white font-bold py-2 px-4 rounded" type="button"
      @click="count++">count is {{ count }}
    </button>
  </div>

</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
