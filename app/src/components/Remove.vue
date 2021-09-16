<template>
<v-container>
    <h2 class="orange--text py-4"> REMOVE STOCK </h2>
    <v-card elevation="2" max-width="450">
        <v-card-text>
            <v-row>
                <v-col>
                    <p> Select a Product Code </p>
                    <v-select
                    :items="products"
                    label=" --Select--"
                    color="orange"
                    solo
                    ></v-select>
                </v-col>
            </v-row>
            <v-row>
                <v-col>
                    <p> Buyer EMail Address </p>
                    <v-text-field
                    dense
                    outlined
                    color="orange"
                    v-model="email"
                    ></v-text-field>
                </v-col>
            </v-row>
            <v-row>
                <v-col>
                    <p> Items Bought </p>
                    <v-text-field
                    dense
                    outlined
                    color="orange"
                    v-model="itemBought"
                    ></v-text-field>
                </v-col>
            </v-row>
            <v-row>
                <v-col align="right">
                    <v-btn raised large block class="orange black--text"> REMOVE STOCK </v-btn>
                </v-col>
            </v-row>
        </v-card-text>   
    </v-card>
</v-container>
</template>

<script>
  export default {
    name: 'Remove',
    data() {
        return{
            products: [
                'PRODUCT01',
                'PRODUCT02',
                'PRODUCT03'
            ],
            itemBought: '',
            email: ''

        }
    }
  }
</script>
<style scoped>
</style>
