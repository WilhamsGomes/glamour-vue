<template>
    <div id="PageInicial">
        <section class="intro-section" id="home">
          <v-row class="align-center justify-space-around px-12 mb-16" >
                    <v-col lg="6" cols="6" class="pa-6 py-16">
                        <Window/>
                        <v-btn href="https://web.whatsapp.com/" target="_blank" id="button" class="ml-16 mb-16" rounded color="white" dark outlined>Entrar em contato</v-btn>
                    </v-col>
                    <v-col lg="6" cols="6" class="d-flex">
                        <img id="foto" class="ml-16" src="../assets/FotoInicial.png" width="450" alt="Foto Formando"/>      
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
        return {};
    },
    components: { 
        Window 
    }
}
    
</script>

<style scoped>

#PageInicial{
    margin-top: 50px;
    z-index: 30 !important;
}    

#foto{
    z-index: 30 !important;
}

@media screen and (max-width: 600px) {

    #button{
        position: absolute !important; 
        margin-left: -40px !important;
    }

    #foto{
        width: 360px;
        margin-top: 15px;
        margin-left: -40px !important;
    }

}

</style>