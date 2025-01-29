<template>
  <div class="home">

    <h1 class="p-8">Home</h1>

    <Welcome msg="Naren Vue3 + Vue + TS 2025 Starter" />

    <button @click="goToAbout">Go to About</button>
  </div>
</template>

<script lang="ts">
import Welcome from '../components/Welcome.vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Home',
  components: {
    Welcome
  },
  methods: {
    goToAbout() {
      this.$router.push('/about');
    }
  }
});
</script>
