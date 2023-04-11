<template>
  <v-responsive class="d-flex align-center text-center">
    <form @submit.prevent="submitForm">

    <v-card>
      
      <v-img src="@/assets/port.jpg" height="200px" cover></v-img>

      <v-card-title> Do you have a product that is on Backorder? </v-card-title>
      <v-card-subtitle> Let us know about it here. </v-card-subtitle>

      <v-card-text>
        Please provide us with the product name, current manufacturers,
        dimensions, specifications and any other information you have.<br /><br />
        The more detail you can provide us with the better!<br /><br />
        We will review your needs and have a Backorder Specialist reach out to
        discuss a variety of solutions to meet your needs.
      </v-card-text>
    </v-card>
    <v-card>
      <v-card-text>

       
        <v-text-field label="Name"  v-model="Name" required></v-text-field>
        <v-text-field label="Product Name"  v-model="productname" required></v-text-field>
        <v-text-field label="Current Manufacturers" v-model="CurrentManufacturers" required></v-text-field>
        <v-text-field label="Dimensions" v-model="Dimensions" required></v-text-field>
        <v-text-field label="Specifications" v-model="Specifications" required></v-text-field>
        <v-textarea label="Other Information" v-model="OtherInformation"> </v-textarea>

      </v-card-text>
      <v-card-actions>
        <v-spacer></v-spacer>
        <v-btn color="#5473fc" size="x-large" variant="flat" type="submit">Submit</v-btn>
        <v-spacer></v-spacer>
      </v-card-actions>
    </v-card>
  </form>

  </v-responsive>
</template>

<script >
import axios from 'axios';

export default {
  data() {
    return {
      Name: '',
      productname: '',
      CurrentManufacturers: '',
      Dimensions: '',
      Specifications: '',
      OtherInformation: '',
      endpoint: 'https://formspree.io/xoqzplll',
    }
  },
  methods: {
    async submitForm() {
      const data = {
        name: this.Name,
        productname: this.productname,
        CurrentManufacturers: this.CurrentManufacturers,
        Dimensions: this.Dimensions,
        Specifications: this.Specifications,
        OtherInformation: this.OtherInformation
      }
      const response = await axios.post(this.endpoint, data)
    },
  },
}
</script>
