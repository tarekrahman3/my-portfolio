<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="container">
    <nav class="flex justify-between items-center">
      <section class="flex flex-col justify-start items-end">
        <p class="text-xl">// rijvy</p>
        <p class="text-sm text-blue-700">web dev</p>
      </section>
      <section class="nav-items">
        <RouterLink class="px-7" to="/">_home</RouterLink>
        <RouterLink class="px-7" to="/about">_about</RouterLink>
        <RouterLink class="px-7" to="/portfolio">_portfolio</RouterLink>
        <RouterLink class="px-7" to="/services">_services</RouterLink>
        <RouterLink class="px-7" to="/resume">_resume</RouterLink>
        <RouterLink class="pl-7" to="/contact">_contact</RouterLink>
      </section>
      <section class="visit-blog"></section>
    </nav>
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" /> -->
  </header>
  <RouterView />
</template>

<style scoped>
.nav-items > a {
  transition: transform 0.2s;
}
.nav-items > a:hover {
  transform: scale(1.2);
}
</style>
