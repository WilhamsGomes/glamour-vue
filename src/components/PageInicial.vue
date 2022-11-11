<template>
    <div id="PageInicial">
        <section class="intro-section" id="home">
          <v-row class="align-center justify-space-around px-12 mb-16" >
                    <v-col lg="6" cols="6" class="pa-6 py-16">
                        <Window id="titleInicial"/>
                        <v-btn href="https://web.whatsapp.com/" target="_blank" id="button" class="ml-16 mb-16" rounded color="white" dark outlined>Entrar em contato</v-btn>
                    </v-col>
                    <v-col cols="6" >
                        <v-img
                            id="foto"
                            :src="linkSrc"
                            max-width="450"
                            min-width="250"
                        >    
                        </v-img>
                         
                    </v-col>
            </v-row>
        </section>
    </div>
</template>

<script>
import Window from './Window.vue';

    export default {
    name: "PageInicial",
    data() {
        return {
            linkSrc: require('@/assets/FotoInicial.png'),
        };
    },
    components: { 
        Window 
    }
}
    
</script>

<style scoped>

#titleInicial{
    min-width: 700px;
    min-height: 200px;
}

#PageInicial{
    margin-top: 50px !important;
    z-index: 30 !important;
}    

#foto{
    z-index: 30 !important;
}

@media screen and (max-width: 900px) {
    #button{
        position: absolute !important; 
        margin-left: -40px !important;
    }

    #foto{
        margin-top: 100px;
        margin-left: -15px !important;
    }

    #titleInicial{
        min-width: 400px;
    }

    #PageInicial{
        margin-top: -10px;
    }
}

@media screen and (min-width: 601px) and (max-width: 800px) {
    #titleInicial{
        min-width: 400px;
    }

    #PageInicial{
        margin-top: -10px;
    }
}

@media screen and  (min-width: 801px) and (max-width: 900px) {
    #button{
        margin-left: -30px !important;
    }
}

@media screen and  (min-width: 901px) and (max-width: 1300px) {
    #titleInicial{
        min-width: 400px;
        min-height: 250px;
        margin-bottom: 20px !important;
    }
}

</style>