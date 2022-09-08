<template>
    <div class="numbers">
        <v-card max-width="100%" class="mx-auto" color="#125C07">
            <v-container>
            <v-row dense>
                <v-col cols="12" style="display: flex; align-items: center; justify-content:space-around;" >
                    <div class="display">
                        <v-card-title class="text-h3 white--text font-weight-bold counter" id="number" data-target="637"> +637 </v-card-title>
                        <v-card-subtitle class="text-subtitle-1 white--text" id="text">Turmas satisfeitas</v-card-subtitle>
                    </div>    
                    <div class="display">
                        <v-card-title class="text-h3 white--text font-weight-bold counter" id="number" data-target="16562"> +16562 </v-card-title>
                        <v-card-subtitle  class="text-subtitle-1 white--text" id="text">Clientes felizes</v-card-subtitle>
                    </div>  
                    <div class="display">
                        <v-card-title class="text-h3 white--text font-weight-bold counter" id="number" data-target="15000"> +15000 </v-card-title>
                        <v-card-subtitle  class="text-subtitle-1 white--text" id="text">Sonhos realizados</v-card-subtitle>
                    </div>             
                   
                </v-col>
            </v-row>
            </v-container>
        </v-card>
    </div>
</template>

<script>

    export default {
        name: "Numbers",

        data(){
            return{
                number:0,
            }
        },

        mounted(){
            
            const counters = document.querySelectorAll('.counter');

            counters.forEach(counter => {
            counter.innerText = '0';

            const updateCounter = () =>{
                const target = +counter.getAttribute('data-target');
                const c = +counter.innerText;

                const increment = target / 600;
                
                if (c < target){
                    counter.innerText = "+"+`${Math.ceil(c + increment)}`;
                    setTimeout(updateCounter, 1);
                } else {
                    counter.innerText = "+"+target;
                }

            }
            updateCounter();
            });

        },

        methods:{
            
            updateNumber(){

            
                
            }

        }
    
    }
</script>

<style scoped>

.display{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

.numbers{
    z-index: 999999999999;
    margin-top: -100px;
}

@media screen and (max-width: 600px) {

    #number{
        font-size: 25px !important;
    }

    #text{
        font-size: 12px !important;
    }

}

</style>