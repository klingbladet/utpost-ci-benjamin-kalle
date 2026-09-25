<script setup>
import { RouterLink, RouterView } from 'vue-router'
import {kallebajsmacka} from 'bajsmacka'
</script>

<template>
  <header>
    <RouterLink to="/guider">Utpost</RouterLink>
  </header>
  <main>
    <RouterView />
  </main>
</template>
