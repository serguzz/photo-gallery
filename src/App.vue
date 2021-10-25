<template>
  <v-app>
    <Navbar/>

    <v-card class="overflow-hidden">
      <v-sheet
        id="scrolling-techniques-3"
        class="overflow-y-auto"
        max-height="600"
      >
        <v-container style="height: 1000px;">

        </v-container>

      </v-sheet>

    </v-card>

    <v-main>
  
    </v-main>
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
