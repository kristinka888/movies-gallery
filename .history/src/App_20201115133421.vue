<template>
  <div id="app">
    <div>
     <router-link to="/"> Головна сторінка</router-link>
     <router-link to="/all_movies"> Список фільмів </router-link>
     <router-link to="/add_movie"> Додати фільм </router-link>
    </div>
    <div>
     <router-view/>
    </div>
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
