<template>
      <v-app-bar
        absolute
        color="#6A76AB"
        dark
        shrink-on-scroll
        prominent
        src="https://picsum.photos/1920/1080?random"
        fade-img-on-scroll
        scroll-target="#scrolling-techniques-3"
      >
        <template v-slot:img="{ props }">
          <v-img
            v-bind="props"
            gradient="to top right, rgba(100,115,201,.7), rgba(25,32,72,.7)"
          ></v-img>
        </template>
  
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
  
        <v-app-bar-title>Photo Gallery</v-app-bar-title>
  
        <v-spacer></v-spacer>
  
        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
  
        <v-btn icon>
          <v-icon>mdi-heart</v-icon>
        </v-btn>
  
        <v-btn icon>
          <v-icon>mdi-dots-vertical</v-icon>
        </v-btn>
  
        <template v-slot:extension>
          <v-tabs align-with-title>
            <v-tab>Home</v-tab>
            <v-tab>Gallery</v-tab>
            <v-tab>Contact</v-tab>

            <v-spacer/>
            <v-btn class="orange mr-1">Home</v-btn>
            <v-btn class="orange mr-1">Callery</v-btn>

          </v-tabs>
        </template>


      </v-app-bar>
    
</template>

<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
    setup() {
        
    },
})
</script>

<style scoped>

</style>
