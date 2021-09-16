<template>
  <v-app id="inspire">
    
    <v-app-bar clipped-left app class="app">
      <v-icon large class="orange--text"> mdi-chart-bar-stacked </v-icon>
      <v-toolbar-title class="ml-2"> STOCK SYSTEM </v-toolbar-title>
    </v-app-bar>

    <v-main>
      <router-view> </router-view>
    </v-main>

  </v-app>
</template>

<script>
  export default {
    name: 'App',
    data(){
      return {
      }
    }
  }
</script>
<style scoped>

</style>