<template>
<v-container>
    <h2 class="orange--text py-4"> STOCK LEVELS </h2>
    <v-card elevation="2" max-width="450">
        <v-card-text>
            <v-list>
              <v-list-item>
                <v-list-item-content>
                  <v-row>
                    <v-col>
                      <v-list-item-title> PRODUCT01 </v-list-item-title>
                      <v-list-item-subtitle> prod </v-list-item-subtitle>
                    </v-col>
                    <v-col align="right">
                      <p> num </p>
                    </v-col>
                  </v-row>
                </v-list-item-content>
              </v-list-item>
              <v-divider> </v-divider>
              <v-list-item>
                <v-list-item-content>
                  <v-row>
                    <v-col>
                      <v-list-item-title> PRODUCT02 </v-list-item-title>
                      <v-list-item-subtitle> text </v-list-item-subtitle>
                    </v-col>
                    <v-col align="right">
                      <p> num </p>
                    </v-col>
                  </v-row>
                </v-list-item-content>
              </v-list-item>
              <v-divider> </v-divider>
              <v-list-item>
                <v-list-item-content>
                  <v-row>
                    <v-col>
                      <v-list-item-title> PRODUCT03 </v-list-item-title>
                      <v-list-item-subtitle> text </v-list-item-subtitle>
                    </v-col>
                    <v-col align="right">
                      <p> num </p>
                    </v-col>
                  </v-row>
                </v-list-item-content>
              </v-list-item>
            </v-list>
        </v-card-text>   
    </v-card>
</v-container>
</template>

<script>
  export default {
    name: 'Dashboard',
    props:{
        product: Object
    },
    data() {
        return{
        }
    },
    mounted(){
    }
  }
</script>
<style scoped>
</style>
