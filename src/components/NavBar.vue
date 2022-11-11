<template> 
    <div class="app">
        <v-app-bar app color="#34B450" flat class="justify-center">  
            <v-img :src="srcLogo"
                max-height="50"
                max-width="120"
            ></v-img>
            <v-tabs centered id="nav-bar-titles" color="#fff" dark>
                <v-tab to="">Home</v-tab>
                <v-tab to="">Eventos</v-tab>
                <v-tab to="">Serviços</v-tab>
                <v-tab to="">Contato</v-tab>
            </v-tabs> 
            
            <v-btn v-for="icon in icons" :key="icon" class="mx-2" dark icon id="icons">
                <v-icon size="20px">
                {{ icon }}
                </v-icon>
            </v-btn>
        </v-app-bar>
    </div>
</template>

<script>
    export default {
        name: "NavBar",
        data: () => ({
            icons: [
                'mdi-youtube',
                'mdi-instagram',
            ],
            srcLogo: require("../assets/GLAMOURPNG.png"),
        }),
    }
</script>

<style scoped>

*{
    color: #fff;
}

#app{
    z-index: 10 !important;
    overflow-x: hidden !important;
}

.app::before{
    content: '';
    position: absolute;
   
    width: 950px;
    height: 800px;
    border-bottom-right-radius: 25px;
    background-color: #34B450;
    transform: skewY(-380deg);
    top: -250px;
   
} 

@media screen and (max-width: 650px) {

    #icons{
       display: none !important;
    }

}

@media screen and (max-width: 550px) {

    .v-tab{
        font-size: 0.675rem !important;
    }

}

</style>