<template>
  <v-container>
    <v-row>
      <v-col>
        <Add :product="product" />
      </v-col>
      <v-col>
        <Dashboard />
      </v-col>
      <v-col>
        <Remove />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  import Dashboard from '@/components/Dashboard'
  import Add from '@/components/Add'
  import Remove from '@/components/Remove'

  export default {
    name: 'Home',
    components: {
      Dashboard,
      Add,
      Remove
    },
    data(){
      return{
        product: {}
      }
    },
    methods:{

    },
    mounted(){
      console.log(this.product);
    }
  }
</script>
