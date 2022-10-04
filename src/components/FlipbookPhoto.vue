<template>
    <div>
        <Flipbook class="flipbook"  :pages="pages" :startPage="1" :clickToZoom="false"/>
    </div>
</template>

<script>

    import Flipbook from 'flipbook-vue/vue2'
    

    export default {
        name:"FlipbookPhoto",
        components: { 
            Flipbook 
        },
       data(){
        return{
            pages: [
                null,
                'https://ts1.github.io/flipbook-vue/images/1.jpg',
                'https://ts1.github.io/flipbook-vue/images/4.jpg',
                'https://ts1.github.io/flipbook-vue/images/5.jpg',
                'https://ts1.github.io/flipbook-vue/images/6.jpg',
            ]
        }
       }
    }
</script>

<style scoped>
    html, body {
        margin: 0;
        padding: 0;
    }
    .flipbook {
        width: 100vw;
        height: 100vh;
        margin-bottom: 50px;
    }
</style>