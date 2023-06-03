

<template>
  <header>

    <div class="wrapper">


      <nav class="">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
      </nav>
    </div>
  </header>

  <router-view />
</template>

<script setup>
import {RouterLink, RouterView} from 'vue-router'</script>

<style lang="sass" scoped>

</style>
