<template>
  <v-app-bar>
    <v-btn icon to="/">
    <v-avatar  size="x-large" >
      <v-img  src="@/assets/logo.jpg" />
    </v-avatar>
  </v-btn>

    <v-app-bar-title> </v-app-bar-title>
    <v-spacer></v-spacer>
    <v-btn to="/Request"  variant="flat" color="#5473fc">
      Backorder Request
    </v-btn>

    <v-btn to="/ContactUs"  variant="flat" color="black" class="ml-2">
      Contact Us
    </v-btn>
  </v-app-bar>
</template>

<script setup>
//
</script>
