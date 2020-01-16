<template>
  <div>
    <v-row no-gutters>
      <v-col
        cols="12"
        sm="6"
        md="8"
      >
        <v-card
          class="pa-2"
          flat
        >
          <p class="display-3">About</p>
          <Carousels/>
        </v-card>
      </v-col>
      <v-col
        cols="6"
        md="4"
      >
        <v-card
          class="pa-2"
          flat
        >
          <card></card>
          <card style="margin-top:20px"></card>
        </v-card>
      </v-col>
    </v-row>
    <v-row no-gutters>
      <v-col
        cols="4"
        md="4"
      >
        <card></card>
      </v-col>
      <v-col
        cols="4"
        md="4"
      >
        <card></card>
      </v-col>
      <v-col
        md="4"
      >
        <card></card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import Carousels from '@/components/Carousels.vue'
import Card from '@/components/Card.vue'

export default {
  name: 'About',
  components: {
    Card,
    Carousels
  }
}
</script>

<style>

</style>
