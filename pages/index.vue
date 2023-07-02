<template>
  <v-card
    class="mx-auto"
  >
    <v-layout>
      <v-app-bar
        color="primary"
      >
        <template v-slot:prepend>
          <v-app-bar-nav-icon></v-app-bar-nav-icon>
        </template>

        <v-app-bar-title>Posts</v-app-bar-title>

        <template v-slot:append>
          <v-btn icon="mdi-dots-vertical"></v-btn>
        </template>
      </v-app-bar>
    </v-layout>
    <v-main>
        <v-container max-width="800" fluid>
          <v-row dense>
            <v-col
              v-for="n in 4"
              :key="n"
              cols="4"
              gap="10"
            >
              <Card />
            </v-col>
          </v-row>
        </v-container>
      </v-main>
  </v-card>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
})
</script>
