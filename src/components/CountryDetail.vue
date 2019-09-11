<template>
  <article v-if="country">
    <p>Name: {{ country.name }}</p>
    <p>Capital: {{ country.capital }}</p>
    <p>Population: {{country.population }}</p>
  </article>
</template>

<script>
export default {
  name: 'country-detail',
  props: ['country']
}
</script>

<style>

</style>