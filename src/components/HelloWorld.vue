<template>
  <v-container class="fill-height">
    
    <v-responsive class="d-flex align-center text-center fill-height">
      <div class="font-weight-medium mb-n1">Welcome to</div>
      <v-img contain height="400" src="@/assets/intiallogo.jpg" />
      <div class="py-1" />

      <div class="font-weight-bold mb-n1">
        Where we specialize in providing solutions for disposal items on
        backorder in the medical field. Our team works with manufacturers and
        suppliers worldwide to ensure that you have access to the products you
        need in a timely manner.<br /><br />
        If you have a product on backorder, visit our "Backorder Requests" page
        to provide us with detailed information, and our Backorder Specialists
        will work with you to find a solution. <br /><br />For any other
        inquiries, please visit our "Contact Us" page and send us an email with
        your contact information. A team member will be in touch with you
        promptly.
      </div>
      <div class="py-4" />
      <v-row class="d-flex align-center justify-center">
        <v-col cols="auto">
          <v-btn
            to="/Request"
            min-width="228"
            size="x-large"
            variant="flat"
            color="#5473fc"
          >
            <v-icon icon="mdi-speedometer" size="large" start />
            Backorder Request
          </v-btn>
        </v-col>
        <v-col cols="auto">

    <v-btn to="/ContactUs"              size="x-large"
 variant="flat" color="black" class="ml-2">
      Contact Us
    </v-btn>
        </v-col>
      </v-row>
    </v-responsive>
  </v-container>
</template>

<script setup>
//
</script>
