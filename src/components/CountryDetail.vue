<template>
  <article v-if="country">
    <p>Name: {{ country.name }}</p>
    <p>Capital: {{ country.capital }}</p>
    <p>Population: {{country.population }}</p>
    <p v-for="(language) in country.languages" v-bind:key="language.name">Language: {{ language.name }}</p>
    <img class="flag" v-bind:src="country.flag" alt="Flag">
  </article>
</template>

<script>
export default {
  name: 'country-detail',
  props: ['country']
}
</script>

<style lang="css" scoped>
  .flag {
    width: 100px;
  }
</style>