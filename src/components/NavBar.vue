<template> 
    <div class="app">
        <v-app-bar app color="#34B450" flat>  
            <img src="../assets/GLAMOURPNG.png" width="100px"/>
            <v-tabs centered class="ml-n9" color="#fff" dark>
                <v-tab to="">Home</v-tab>
                <v-tab to="">Eventos</v-tab>
                <v-tab to="">Serviços</v-tab>
                <v-tab to="">Contato</v-tab>
            </v-tabs>
            
            <v-btn v-for="icon in icons" :key="icon" class="mx-2" dark icon >
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
                'mdi-facebook',
                'mdi-youtube',
                'mdi-instagram',
            ],
        }),
    }
</script>

<style scoped>

*{
    color: #fff;
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

</style>