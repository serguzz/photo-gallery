<template>
  <v-app>
    
    
    <v-card class="overflow-hidden">
      <v-sheet
        id="scrolling-techniques-3"
        class="overflow-y-auto"
        max-height="600"
      >
        <v-container style="height: 500px;">
          <Navbar/>
          <router-view/>
        </v-container>
      
        <router-view/>
      </v-sheet>

    </v-card>

    <v-main>
      <router-view/>
    </v-main>
    <router-view/>
  </v-app>
</template>

<script>

import Navbar from "@/components/Navbar";
export default {
  name: 'App',

  components: {
    Navbar
  },

  data: () => ({
    //
  }),
};
</script>
