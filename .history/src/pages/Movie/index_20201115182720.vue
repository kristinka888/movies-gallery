<template>
    <div>
      <b-button-group size="lg">
       <b-button to="/" variant="light">Головна сторінка</b-button>
       <b-button to="/all_movies" variant="light">Список фільмів</b-button>
       <b-button to="/add_movie" variant="light">Додати фільм</b-button>
       </b-button-group>
       <movie-details/>
    </div>
</template>

<script>
import MovieDetails from "../../components/MovieDetails"
    export default {
        name:"Movie",
        components: {
            MovieDetails,
        },
    }
</script>

<style lang="scss" scoped>

</style>