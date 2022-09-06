<template>
    <div class="app">
        <v-app-bar app color="#34B450" flat >  
            <v-tabs centered class="ml-n9" color="#fff" dark>
                <v-tab to="">Home</v-tab>
                <v-tab to="">Eventos</v-tab>
                <v-tab to="">Serviços</v-tab>
                <v-tab to="">Contato</v-tab>
            </v-tabs>
        </v-app-bar>
    </div>
    
</template>

<script>
    export default {
        name: "NavBar",
        
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