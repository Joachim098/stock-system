<template>
  <v-container>
    <v-row>
      <v-col>
        <Dashboard />
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
  import Dashboard from '@/components/Dashboard'
  export default {
    name: 'Home',
    components: {
      Dashboard
    }
  }
</script>
