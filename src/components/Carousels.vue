<template>
    <v-carousel
      hide-delimiters
    >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    >
      <v-sheet
        height="100%"
        color="rgba(0, 0, 0, 0.3)"
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <div class="text-center" style="width:70%">
            <p class="display-2">{{item.title}}</p>
            <p class="display-1">{{item.subTitle}}</p>
            <v-btn depressed color="deep-orange" class="mt-8">Normal</v-btn>
          </div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data () {
    return {
      items: [
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          title: 'Themes',
          subTitle: 'Vuetify Material Dashboard PRO Theme'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          title: 'Themes2',
          subTitle: '2Vuetify Material Dashboard PRO Theme'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
          title: 'Themes3',
          subTitle: '3Vuetify Material Dashboard PRO Theme'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          title: 'Themes4',
          subTitle: '4Vuetify Material Dashboard PRO Theme'
        }
      ]
    }
  }
})
</script>

<style scoped>

</style>
