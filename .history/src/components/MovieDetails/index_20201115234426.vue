<template>
    <div>
        <b-card class="mx-auto"
        :title='getMovie.name'
        :img-src='getMovie.image'
        img-alt="movie-image"
        style="max-width: 19rem;"
        img-top
        >
        <b-card-text>
            Жанр:{{getMovie.genre}}<br/>
            Рік:{{getMovie.year}}<br/>
            Країна:{{getMovie.country}}<br/>
            Актори:{{getMovie.actors}}<br/>
            Тривалість фільму:{{getMovie.duration}} хв
        </b-card-text>
        </b-card>
      </div>
</template>

<script>
    export default {
        name:"MovieDetails",
        props: {
             movieId: {
                type: [String,Number],
                required:true
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