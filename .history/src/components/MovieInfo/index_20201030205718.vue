<template>
    <div>
       <div> {{name}}</div>
       <div> <img :src="image" alt="movie-image" /></div>
       <div> Жанр:{{genre}}</div>
       <div> Рік:{{year}}</div>
       <div> Тривалість:{{duration}}</div>
       <div>
           Актори:{{actors}}
       </div>
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
                required:true
            },
            image:{
                type:String,
                default:require('@/../../assets/images/no-image-logo.jpg')
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
            }

        },
    }
</script>

<style lang="scss" scoped>

</style>