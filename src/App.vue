<template>
  <v-app>
    <v-app-bar app color="primary">
      <!-- -->
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <hello-world />
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
import { HelloWorld } from "@frylock34/hello-world"

@Component({
  components: {
    HelloWorld
  }
})
export default class App extends Vue { }
</script>

<style>
</style>
