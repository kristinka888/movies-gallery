<template>
    <div>
       <div> {{name}}</div>
       <div> <img :src="image" alt="movie-image" /></div>
       <div> {{year}}</div>
    </div>
</template>

<script>
    export default {
        name:"MovieInfo",
        props: {
            id: {
                type: [String,Number],
                required:true,
            },
            name:{
                type:String,
                default:"Назва відсутня",
            },
            image:{
                type:String,
                default:require("@/assets/images/no-image-logo.jpg")
            },
            year:{
                type:[String,Number],
                default:"Немає року випуску"
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>