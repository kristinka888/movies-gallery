<template>
    <div>
        <b-button-group vertical class="mx-auto bg-info" width="400px">
        <b-button variant='light' size="lg">
       <router-link to="/all_movies">Перейти до списку фільмів</router-link>
       </b-button>
       <b-button variant='light' size="lg">
       <router-link to="/add_movie">Додати фільм</router-link>
       </b-button>
        </b-button-group>
   </div>
</template>

<script>
 export default {
        name:"Home",
        components:{
           
        }
    }
</script>

<style lang="scss" scoped>

</style>