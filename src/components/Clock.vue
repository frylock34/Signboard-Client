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
  mounted () {
    this.handler = window.setInterval(() => {
      let now = new Date();
    })

  }
  beforeDestroy () {
    window.clearTimeout();
  }

  handler: any

  hours: number = 0

  minutes: number = 0

  seconds: number = 0
}

</script>

<style>
</style>