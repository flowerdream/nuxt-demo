<template>
    <div class="movie-type">
        <nuxt-link 
            v-for="item in movieList"
            :key="item.id"
            :to="`/movie/${$route.params.type}/${item.id}`"
            class="movie-box"
        >
        <h4>电影名:{{item.name}}</h4>
        <p>电影ID:{{item.id}}</p>
        <img :src="item.img">
        </nuxt-link>
    </div>
</template>
<script>
    import axios from 'axios'
    export default {
        layout: "movie",
        // head(){
        //     return {
        //         meta: [
        //             {
        //                 name: "keyword",
        //                 content: "电影"
        //             }
        //         ]
        //     }
        // },
        asyncData(content ) {
            return axios.get('http://localhost:3000/comments').then( res => {
                return {movieList: res.data};
            })
        }
    }
    
</script>
<style>
    .movie-type{
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .movie-box{
        display: flex;
        flex-direction: column;
        align-items: center;
        margin: 20px 0;
        padding: 10px 0;
        width: 40%;
        box-shadow: 0 0 10px #bbb;
    }
</style>