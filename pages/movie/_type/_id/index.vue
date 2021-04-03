<template>
    <div class="movie">
       详情页面{{type }}{{id}}
    </div>
</template>
<script>
    export default {
        layout: "movie",
        asyncData(context) {
            return {type:context.route.params.type, id:context.route.params.id}
        }
    }
    
</script>