<template>
  <v-app-bar>
    <v-btn icon to="/">
    <v-avatar  size="x-large" >
      <v-img  src="@/assets/logo.jpg" />
    </v-avatar>
  </v-btn>

    <v-app-bar-title> </v-app-bar-title>
    <template v-slot:append>
          <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
        </template>
    <v-spacer></v-spacer>

  </v-app-bar>
  <v-navigation-drawer
        v-model="drawer"
        location="right"
        temporary
      >
        
        <v-list-item v-for="(i,j) in items" :key="j"
            :title="i.title"
            :to="i.Value"
            
          ></v-list-item>
      
      </v-navigation-drawer>
</template>

<script >
 export default {
    data: () => ({
      drawer: false,
      items: [
      {title: 'Home', Value: '/'},
        {title: 'Backorder Request', Value: 'Request'},
        {title: 'Contact Us', Value: 'ContactUs'},
      ],
    }),

    watch: {
      
    },
  }
</script>
