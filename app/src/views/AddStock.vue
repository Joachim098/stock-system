<template>
<v-container>
    <v-row>
      <v-col>
        <Add />
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
  import Add from '@/components/Add'
  export default {
    name: 'AddStock',
    components: {
      Add
    },
  }
</script>
