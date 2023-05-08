<template>
  <v-container class="fill-height">
    <v-responsive class="d-flex align-center text-center fill-height">
      <div class="font-weight-medium mb-n1">Welcome to</div>
      <v-img contain height="400" src="@/assets/logo.jpg" />
      <div class="py-1" />

      <div class="font-weight-bold mb-n1">
        Backorder Solutions is a US-based company dedicated to providing medical
        facilities with effective solutions amidst current supply constraints.
        Through our partnership with a trusted manufacturing company boasting
        over two decades of experience in producing pneumatic tourniquet cuffs,
        we offer exceptional manufacturing equipment and capabilities, including
        the ability to create different molds. 
        
        <br /><br />
        Our products undergo Cobalt 60
        radiation sterilization and are manufactured in a 100,000-level
        purification workshop. We hold several patented technologies and can
        customize our products to suit the unique needs of our clients. We
        maintain strict adherence to ISO13485 and ISO14001 standards in all our
        production processes.
        <br /><br />
        Where we specialize in providing solutions for
         products on backorder in the medical field. Our team works with
        manufacturers and suppliers worldwide to ensure that you have access to
        the products you need in a timely manner.<br /><br />
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
          <v-btn
            to="/ContactUs"
            size="x-large"
            variant="flat"
            color="black"
            class="ml-2"
          >
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
