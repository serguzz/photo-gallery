<template>
    <v-container>

        <v-row>
            <Photo
                v-for="photo in photos"
                v-bind:photo="photo"
            
            />

        </v-row>
    </v-container>
</template>

<script>

import axios from 'axios'
import Photo from "@/components/photo/Photo"

export default {
    
 

    components: {
        Photo
    },

    data: () => ({
        photos: [
            { id: 1, title: 'photo 1'},
            { id: 2, title: 'photo 1'},
            { id: 3, title: 'photo 1'},
            { id: 4, title: 'photo 1'},
            
        ]
    }),

    mounted() {
       this.fetchPhotos()
 //      setTimeout(() => {this.photos = [ { id: 4, title: 'photo 1'},]}, 1000)
    },

    methods: {
        fetchPhotos() {
             axios.get(`https://jsonplaceholder.typicode.com/photos?_limit=10`)
                .then(response => this.photos = response.data)
        }
    }

}
</script>

<style scoped>

</style>