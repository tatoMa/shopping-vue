<template>
  <v-card class="overflow-hidden">
    <v-app-bar
      absolute
      color="blue darken-3"
      dark
      shrink-on-scroll
      height="80px"
      src="https://images.pexels.com/photos/358528/pexels-photo-358528.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
      fade-img-on-scroll
      scroll-target="#scrolling-techniques-3"
      scroll-threshold=200
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(100,115,201,.7), rgba(25,32,72,.7)"
        ></v-img>
      </template>

      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Tato Stores</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-cart-outline</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-account-circle-outline</v-icon>
      </v-btn>

      <template v-slot:extension>
        <v-tabs
          align-with-title
          background-color="transparent"
        >
          <v-tab to="/">HOME</v-tab>
          <v-tab>COLLECTIONS</v-tab>
          <v-tab>CONTACT US</v-tab>
          <v-tab to="/about">ABOUT</v-tab>
        </v-tabs>
      </template>
    </v-app-bar>
    <v-sheet
      id="scrolling-techniques-3"
      class="overflow-y-auto"
    >
      <v-container style="height: 100vh">
        <router-view/>
      </v-container>
    </v-sheet>
  </v-card>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
