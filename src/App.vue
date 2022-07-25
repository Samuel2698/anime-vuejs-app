<script setup>
import { ref, computed, onMounted } from "vue";

const query = ref("");
const my_amine = ref([]);
const search_results = ref([]);

const my_anime_asc = computed(() => {
  return my_anime.value.sort((a, b) => {
    return a.title.localeCompare(b.title);
  });
});

// const searchAnime = () => {
//   const url = `https://api.jikan.moe/v4/anime?q=${query.value}`;
//   fetch(url).then((res) => res.json);
// };
</script>

<template>
  <main>Hello World :)</main>
</template>

<style></style>
