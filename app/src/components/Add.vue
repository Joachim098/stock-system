<template>
<v-container>
    <h2 class="orange--text py-4"> ADD STOCK </h2>
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
                    v-model="selectedProduct"
                    ></v-select>
                </v-col>
            </v-row>
            <v-row>
                <v-col>
                    <p> Items Received </p>
                    <v-text-field
                    dense
                    outlined
                    color="orange"
                    v-model="item"
                    ></v-text-field>
                </v-col>
            </v-row>
            <v-row>
                <v-col>
                    <p> Price per Item Received </p>
                    <v-text-field
                    dense
                    outlined
                    color="orange"
                    v-model="price"
                    ></v-text-field>
                </v-col>
            </v-row>
            <v-row>
                <v-col align="right">
                    <v-btn raised large block class="orange white--text" v-on:click="addProduct"> ADD STOCK </v-btn>
                </v-col>
            </v-row>
        </v-card-text>   
    </v-card>
</v-container>
</template>

<script>
  export default {
    name: 'Add',
    props:{
        product: Object
    },
    data() {
        return{
            products: [
                'PRODUCT01',
                'PRODUCT02',
                'PRODUCT03'
            ],
            selectedProduct: '',
            item: '',
            price: ''

        }
    },
    methods: {
        addProduct(){
            if (this.selectedProduct == '' || this.item == '' || this.price == ''){
                alert("Please make sure you fill in all the fields");
            }
            else{
                this.proctuct = {
                    selectedProduct: this.selectedProduct,
                    items: this.item,
                    price: this.price
                }
              alert("Stock has been added"); 
              console.log(this.proctuct);
              this.selectedProduct = '',
              this. item = '',
              this. price = ''
            }
        }
    },
    mounted(){
    }
  }
</script>
<style scoped>
</style>
