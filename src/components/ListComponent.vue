<template>
  <li>{{ country.name }}</li>
</template>

<script>
import { eventBus } from '../main.js'

export default {
  name: 'list-component',
  props: ['country'],
}
</script>

<style>

</style>