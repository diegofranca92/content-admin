<template>
  <nav>
    <v-bottom-navigation>
      <NuxtLink to="app/list">
        <v-btn value="recent">
          Lista
          <v-icon>mdi-history</v-icon>
        </v-btn>
      </NuxtLink>
      <NuxtLink to="app/cadastro">
        <v-btn value="favorites">
          Cadastro
          <v-icon>mdi-heart</v-icon>
        </v-btn>
      </NuxtLink>
    </v-bottom-navigation>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
})
</script>
