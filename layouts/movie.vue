<template>
    <div class="movie-layout">
        <my-header/>
        <nuxt></nuxt>
    </div>
</template>
<script>
    import MyHeader from "~/components/header"
    export default {
        components: {
            MyHeader
        }
    }
</script>
<style>
    .movie-layout{
        margin-top: 60px;
    }
</style>