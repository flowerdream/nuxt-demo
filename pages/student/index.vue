<template>
    <div>
        <div style="margin: 30px; font-size: 30px;">这个是默认路由index</div>
        <nuxt-link to="/student/1" class="button">1</nuxt-link>
        <nuxt-link to="/student/2" class="button">2</nuxt-link>
        <nuxt-link to="/student/3" class="button">3</nuxt-link>
    </div>
</template>
<style>
    .button{
        width: 50px;
        height: 50px;
        margin: 20px;
        background-color: blue;
        color: ivory;
        font-size: 20px;
        display: inline-block;
        text-align: center;
        line-height: 50px;
    }
    .button:hover{
        background-color:red;
    }
</style>