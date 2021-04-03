<template>
    <div class="moverHeader">
        <ul>
            <li>
                <nuxt-link to="/movie/in">正在热映</nuxt-link>
            </li>
            <li>
                <nuxt-link to="/movie/com">即将上映</nuxt-link>
            </li>
            <li>
                <nuxt-link to="/movie/20">top20</nuxt-link>
            </li>
        </ul>
    </div>
</template>
<style scope>
    .moverHeader {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
    }
    ul {
        display: flex;
        justify-content: space-around;
        align-items: center;
        padding: 15px 0;
        background-color: #1e2736;
        margin: 0;
    }
    li {
        list-style: none;
        line-height: 30px;
        height: 30px;
    }
    li a {
        color: white;
    }
    li a:hover {
        color: red;
    }
</style>