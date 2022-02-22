<script setup lang="ts">
const isDark = useDark()
const toggleDark = useToggle(isDark)
</script>

<template>
  <header class="max-w-prose m-auto dark:text-gray-200">
    <h1 class="font-bold text-2xl md:text-4xl mt-10">
      zzw
    </h1>
    <nav class="flex space-x-3 md:space-x-6 mt-6">
      <router-link to="/">
        Home
      </router-link>
      <router-link to="/posts">
        Posts
      </router-link>
      <router-link to="/about">
        About
      </router-link>
      <button class="icon-btn mx-2 !outline-none" @click="toggleDark()">
        <div i="carbon-sun dark:carbon-moon" />
      </button>
    </nav>
  </header>
</template>
