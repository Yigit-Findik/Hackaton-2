<template>
  <header>
    <nav>
      <ul>
        <li><NuxtLink to="/index">Index</NuxtLink></li>
      </ul>
    </nav>
  </header>
</template>

<script setup lang="ts">
const route = useRoute();

// When accessing /taxi-rit/1, route.params.id will be 1 (routes
console.log(route.params.id)
</script>