<template>
  <div id="app">
    <!-- <movie-info name="Lovers" image="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTaZ1JMDsCvFaowUQKz6TLrIiJHqpilkDsDEg&usqp=CAU"
    year=2001 duration=120 genre="Comedy" :actors='["juou","hjyhfg"]'>
    </movie-info> -->
     <router-link to="/"> Головна сторінка</router-link>
     <router-link to="/all_movies"> Список фільмів </router-link>
     <router-link to="/add_movie"> Додати фільм </router-link>
     <router-view/>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
   
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
