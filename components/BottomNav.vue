<template>
  <v-layout class="overflow-visible" style="height: 56px">
    <v-bottom-navigation v-model="value" :bg-color="color" mode="shift" grow>
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
      <NuxtLink to="/">
        <v-btn>
          <span>Sair</span>
          <v-icon>mdi-logout</v-icon>
        </v-btn>
      </NuxtLink>
    </v-bottom-navigation>
  </v-layout>
</template>
<script>
export default {
  data: () => ({ value: 1 }),

  computed: {
    color() {
      switch (this.value) {
        case 0:
          return 'blue-grey'
        case 1:
          return 'teal'
        case 2:
          return 'brown'
        default:
          return 'blue-grey'
      }
    },
  },
}
</script>
