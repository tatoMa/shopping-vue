<template>
  <div class="grey lighten-5 top-space">
    <v-row no-gutters>
      <v-col
        cols="12"
        sm="6"
        md="8"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          <Carousels/>
        </v-card>
      </v-col>
      <v-col
        cols="6"
        md="4"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          <card></card>
          <card></card>
        </v-card>
      </v-col>
    </v-row>
    <v-row no-gutters>
      <v-col
        cols="12"
        sm="6"
        md="8"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          <Carousels/>
        </v-card>
      </v-col>
      <v-col
        cols="6"
        md="4"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          <card></card>
          <card></card>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import Carousels from '@/components/Carousels.vue'
import Card from '@/components/Card.vue'

export default {
  name: 'home',
  components: {
    Card,
    Carousels
  }
}
</script>

<style>
body{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.top-space{
  margin-top: 170px;
}
</style>
