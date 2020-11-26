<template>
  <v-app>
    <v-app-bar app color="primary">
      <!-- -->
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <Clock />
      </v-container>
    </v-main>

    <v-footer app>
      <!-- -->
    </v-footer>
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Clock from '@/components/Clock.vue';

@Component({
  components: {
    Clock
  }
})
export default class App extends Vue { }
</script>

<style>
</style>
