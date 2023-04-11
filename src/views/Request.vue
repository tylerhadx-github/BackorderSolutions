<template>
    <v-responsive class="d-flex align-center text-center">
      <v-card>
        <v-img src="@/assets/port.jpg" height="200px" cover></v-img>

        <v-card-title>
          Do you have a product that is on Backorder?
        </v-card-title>
        <v-card-subtitle> Let us know about it here. </v-card-subtitle>

        <v-card-text>
          Please provide us with the product name, current manufacturers,
          dimensions, specifications and any other information you have.<br><br> The
          more detail you can provide us with the better!<br><br> We will review your
          needs and have a Backorder Specialist reach out to discuss a variety
          of solutions to meet your needs.
        </v-card-text>
      </v-card>
      <v-card>
        <v-card-text>
          <v-text-field
            label="Product Name"
            required
          ></v-text-field>
          <v-text-field
            label="Current Manufacturers"
            required
          ></v-text-field>
          <v-text-field
            label="Dimensions"
            required
          ></v-text-field>
          <v-text-field
            label="Specifications"
            required
          ></v-text-field>
          <v-textarea label="Other Information">
            
          </v-textarea>
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="#5473fc" size="x-large" variant="flat">Submit</v-btn>
          <v-spacer></v-spacer>
        </v-card-actions>
      </v-card>
    </v-responsive>
</template>

<script setup>
</script>
