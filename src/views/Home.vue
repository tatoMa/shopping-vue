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
    <p class="display-3 text-center font-weight-medium my-8">Featured Products</p>
    <v-carousel
    cycle
    height="400"
    hide-delimiter-background
    show-arrows-on-hover
  >
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
      <v-sheet
        :color="colors[i]"
        height="100%"
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <div class="display-3">{{ slide }} Slide</div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
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
  },
  data () {
    return {
      colors: [
        'indigo',
        'warning',
        'pink darken-2',
        'red lighten-1',
        'deep-purple accent-4'
      ],
      slides: [
        'First',
        'Second',
        'Third',
        'Fourth',
        'Fifth'
      ]
    }
  }
}
</script>

<style>

</style>
