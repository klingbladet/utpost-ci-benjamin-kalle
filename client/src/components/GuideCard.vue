<script setup>
defineProps({
  guide: { type: Object, required: true },
})
const kalle = 'denhär kommer skapa kaos'
</script>

<template>
  <article class="card">
    <p>Vem är Kalle? - {{ kalle }}</p>
    <h3>
      <RouterLink :to="`/guider/${guide.slug}`">{{ guide.title }}</RouterLink>
    </h3>
    <p class="muted">{{ guide.region }} · {{ guide.difficulty }} · {{ guide.length_km }} km</p>
  </article>
</template>

<style scoped>
.card {
  border: 1px solid #ddd;
  padding: 12px;
  border-radius: 4px;
}
.muted {
  color: #777;
  font-size: 14px;
}
</style>
