<template>
    <div>
        <div style="margin: 30px; font-size: 30px;">这个教师index</div>
        <nuxt-link to="/teacher/1" class="button">teacher1</nuxt-link>
        <nuxt-link to="/teacher/2" class="button">teacher2</nuxt-link>
        <nuxt-link to="/teacher/3" class="button">teacher3</nuxt-link>
        <!-- 这是一个坑呀 -->
        <!-- <nuxt-child></nuxt-child> -->
    </div>
</template>
<style>
    .button{
        width: 100px;
        height: 100px;
        margin: 20px;
        background-color: blue;
        color: ivory;
        font-size: 20px;
        display: inline-block;
        text-align: center;
        line-height: 100px;
    }
    .button:hover{
        background-color:red;
    }
</style>