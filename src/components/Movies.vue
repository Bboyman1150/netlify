<template>
  <div>
        <h1>Upcoming Movies</h1>
        <p v-for="movie in movies" :key=movie.id>
            {{movie.original_title}}
            <img :src="`https://image.tmdb.org/t/p/w300/${movie.poster_path}`" alt="">
            <router-link :to="` /detail/${movie.id}`"><p>{{movie.id}}</p></router-link>

        </p>
 </div>
</template>

<script>
import axios from 'axios'
export default {
    name:'Movies',
    data()
    {
        return{
            movies:[]
        }
    },
    mounted()
    {
        axios.get("https://api.themoviedb.org/3/movie/now_playing?api_key=70a15c30fb26538a968ba499524a5e4e&language=en-US&page=1").then((response) =>{
            console.log(response.data.results)
            this.movies = response.data.results;
        })
    }

}
</script>

<style>

</style>