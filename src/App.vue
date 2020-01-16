<template>
  <div id="app">
    <v-app>
      <appbar/>
      <!-- <div id="nav">
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link>
      </div> -->
      <!-- <router-view/> -->
    </v-app>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Appbar from '@/components/Appbar.vue'

export default Vue.extend({
  components: {
    Appbar
  }
})
</script>

<style scoped>

</style>
<style lang="scss">
body{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.top-space{
  margin-top: 190px;
}
.z-index-top{
  z-index: 999 !important;
}
</style>
