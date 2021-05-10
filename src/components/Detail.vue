<template>
<div>
    <h1>Movie Detail</h1>
    <p>{{detailObj.title}}</p>
</div>
  
</template>

<script>
import axios from 'axios'
export default {
    name: 'Detail',
    data(){
        return{
            id:this.$route.params.id
        },
        mounted()
        {
            axios.get("https://api.themoviedb.org/3/movie/${movie_id}?api_key=70a15c30fb26538a968ba499524a5e4e&language=en-US").then((response) =>{
                this.detailObj = response.data;
                console.log(response.data)
            })
        }
    }
}
</script>

<style>

</style>