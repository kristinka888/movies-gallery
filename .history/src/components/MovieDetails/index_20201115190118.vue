<template>
    <div>
        {{store.getters.getMovieById(movieId)}}
       <div>{{movieId}}</div>
       <div> {{genre}}</div>
       <div> <img :src="image" alt="movie-image" /></div>
       <div> Жанр:{{genre}}</div>
       <div> Рік:{{year}}</div>
       <div> Тривалість:{{duration}}</div>
       <div> Країна: {{country}}</div>
       <div> Актори:{{actors}}</div>
    </div>
</template>

<script>
import { mapGetters } from 'vuex'
    export default {
        name:"MovieDetails",
        props: {
             movieId: {
                type: [String,Number],
                required:true,
            },
            name:{
                type:String,
                required:true
            },
            image:{
                type:String,
                default:require('../../assets/images/movie-logo.jpg')
            },
            genre:{
                type:String,
                default:"Жанр не вказаний"
            },
            year:{
                type:[String,Number],
                default:"Немає року випуску"
            },
            country:{
                type:String,
                default:"Рік невідомий"
            },
            actors:{
                type:String,
                default:""
            },
            duration:{
                type:[String,Number],
                default:"Тривалість даного фільму невідома"
            },
            
        },
        computed: {
            getMovie() {
                return this.$store.getters.getMovieById(this.movieId)
            }
        },
        
    }
</script>

<style lang="scss" scoped>

</style>