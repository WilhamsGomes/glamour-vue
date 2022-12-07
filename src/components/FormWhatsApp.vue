<template>
    <v-row id="contact-area" class="d-flex justify-center mb-8 mt-8">
        <v-card class="d-block ml-8 pt-8 " elevation="0" width="600px" dark>
            <div class="mb-8">
                <h1 class=" font-weight-bold display-2 text--white" id="font">Entre em contato conosco!</h1>
                <hr/>
            </div>
            <v-form >
                <v-row class="text--white">
                    <v-col cols="12">
                        <v-text-field 
                            color="white"
                            v-model="name"
                            label="Qual seu nome?"
                            required
                            dark
                        ></v-text-field>
                    </v-col>
                    <v-col cols="12">
                        <v-text-field 
                            color="white"
                            v-model="instituicao"
                            label="Qual sua instituição de ensino?"
                            required
                            dark
                        ></v-text-field>
                    </v-col>
     
                    <v-col cols="12">
                        <v-text-field 
                            color="white"
                            v-model="periodo"
                            label="Qual seu ano e semestre de conclusão?"
                            required
                            dark
                        ></v-text-field>
                    </v-col>
                    <v-col cols="12">
                        <v-btn color="green" depressed class=" white--text" @click="messageWhatsApp()">
                            Entrar em contato
                        </v-btn>
                    </v-col>
                </v-row>
            </v-form>
        </v-card>
        <v-card elevation="0" dark class="pb-8">
            <v-img
                :src="linkSrc"
                max-height="550"
                max-width="550"
            ></v-img>
        </v-card>
    </v-row>
</template>

<script>
    export default {
        name:"FormWhatsApp",
        data(){
            return{
                name: '',
                instituicao: '',
                periodo: '',
                linkSrc: require('@/assets/art-forms.png')
            }
        },

        methods:{

            messageWhatsApp(){
                const link = "https://api.whatsapp.com/send?phone=558188690954&text= *Olá, Glamour Assessoria de Eventos. %0A %0A Meu nome é: *"+ this.name + "* %0A %0A, sou aluno da instituição: " + this.instituicao + "*, com previsão de conclusão em " + this.periodo+"! ";
                window.open(link, "_blank")
                //alert("Vamos enviar para o zap")
            }

        }
    }   
</script>

<style >

@import url('https://fonts.googleapis.com/css2?family=Fira+Sans+Condensed&display=swap');

#font{
    font-family: 'Fira Sans Condensed' !important;
}

hr{
    border: none;
    background-image: linear-gradient(to right, #125C07, #125C07);
    width: 350px;
    height: 6px;
    border-radius: 15px;
    margin-top: 10px !important;
}

#contact-area{
    background-color: #1E1E1E;
}

</style>