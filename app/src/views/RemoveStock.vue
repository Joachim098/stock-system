<template>
 <v-container>
    <v-row>
      <v-col>
        <Remove />
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
  import Remove from '@/components/Remove.vue'
  export default {
    name: 'RemoveStock',
    components: {
      Remove
    },
  }
</script>
