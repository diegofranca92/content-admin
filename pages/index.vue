<template>
  <nav>
    <NuxtLink to="/home"> Lista </NuxtLink>
    <NuxtLink to="/cadastro"> Form </NuxtLink>
    <Tutorial />
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
})
</script>
