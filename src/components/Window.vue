<template>
    <div>
        <typical  id="text"
            class="typicalWrapper display-3 white--text font-weight-bold ml-16 mt-16 "
            :steps="['Há 18 anos, a empresa líder em clientes satisfeitos!', 1000, 'Um novo conceito de assessoria para sua formatura!', 1000, 'VEM SER GLAMOUR!', 1000]"
            :loop="Infinity"
            :wrapper="'h2'"
        ></typical>
    </div>
</template>

<script>

    import typical from 'vue-typical';

    export default {
        name:"Window",
        components:{
            typical
        }
    }
</script>

<style scoped>

.typicalWrapper::after {
  content: "|";
  animation: blink 1s infinite step-start;
}

@keyframes blink {
  50% { opacity: 0; }
}


@media screen and  (max-width: 800px) {

    #text{
        position: relative;
        width: 250px !important;
        line-height: 45px;
        font-size: 40px !important;
        margin-left: -40px !important;
    }

}

@media screen and  (min-width: 801px) and (max-width: 900px) {

    #text{
        position: relative;
        width: 250px !important;
        line-height: 45px;
        font-size: 50px !important;
        margin-left: -20px !important;
        margin-bottom: 10px !important;
    }

}

@media screen and (max-width: 600px) {

    #text{
        position: relative;
        width: 250px !important;
        line-height: 45px;
        font-size: 35px !important;
        margin-left: -40px !important;
        margin-bottom: 20px !important;
    }

}


</style>