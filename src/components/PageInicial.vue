<template>
    <div id="PageInicial">
        <section class="intro-section" id="home">
          <v-row class="align-center justify-space-around px-12 mb-16" >
                    <v-col lg="6" cols="6" class="pa-6 py-16">
                        <p id="title" class="display-3 white--text font-weight-bold ml-16 mt-16 mb-16">Há 17 anos, a empresa líder em clientes satisfeitos!</p>
                        <v-btn href="https://web.whatsapp.com/" target="_blank" id="button" class="ml-16 mb-16">Entrar em contato</v-btn>
                    </v-col>
                    <v-col lg="6" cols="6" class="d-flex">
                        <img class="ml-16" src="../assets/moca.png" width="450"/>      
                    </v-col>
            </v-row>
            
        </section>
    </div>
</template>

<script>

    export default {
    name: "PageInicial",
    data() {
        return {};
    },

    mounted(){

        const tituloCliente = document.getElementById('title');
        const textoArray = tituloCliente.innerHTML.split('');
        tituloCliente.innerHTML = '';

        textoArray.forEach( (letra, i) =>{
            setTimeout(function(){ 
                tituloCliente.innerHTML += letra
                tituloCliente.style.color = 'red'
            }, 50 * i) 
        });


    }

}
    
</script>

<style scoped>

#PageInicial{
    margin-top: 50px;
    z-index: 99999;
}    

@media screen and (max-width: 600px) {

    #title{
        width: 250px;
        line-height: 45px;
        font-size: 40px !important;
        margin-left: -40px !important;
    }

    #button{
        margin-left: -40px !important;
    }

}

</style>