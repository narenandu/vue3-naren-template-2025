<template>
  <div id="app">
    <div class="p-8 flex gap-4 justify-center">
      <div class="flex gap-4">
        <router-link to="/">Home</router-link>
      </div>
      <div>
        <router-link to="/about">About</router-link>
      </div>
    </div>
    <router-view />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App'
});
</script>
