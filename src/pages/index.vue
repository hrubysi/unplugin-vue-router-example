<script setup lang="ts">
import {useRouter} from "vue-router/auto";

const router = useRouter();
router.push({name: ''});
</script>

<template>
  <main>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink :to="{name: '/articles/[slug]', params: {slug: 'test'}}">Test article</RouterLink>
  </main>
</template>
