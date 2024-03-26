<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <nav>
      <section class="brand">
        <p>
          // rijvy
          <span>web dev</span>
        </p>
      </section>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/portfolio">Portfolio</RouterLink>
      <RouterLink to="/services">Services</RouterLink>
      <RouterLink to="/resume">Resume</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
      <section class="visit-blog"></section>
    </nav>
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" /> -->
  </header>
  <RouterView />
</template>

<style scoped>
nav {
  display: flex;
  align-items: center;
  justify-content: center;

  .brand {
    font-size: large;
    span {
      font-size: small;
    }
  }

  a {
    padding: 0px 20px;
  }
}
</style>
