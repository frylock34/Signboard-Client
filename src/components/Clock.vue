<template>
  <v-card>
    <v-container>
      <v-row>
        <v-col cols="12">
          <div class="text-h1">{{ hours }}:{{ minutes }}: {{ seconds }}</div>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'

@Component
export default class Clock extends Vue {
  get hours (): number {
    return new Date().getHours()
  }

  get minutes (): number {
    return new Date().getMinutes()
  }

  get seconds (): number {
    return new Date().getSeconds()
  }
}

</script>

<style>
</style>