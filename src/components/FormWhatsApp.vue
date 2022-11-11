<template>
    <v-row class="justify-center">
        <v-col cols="6" >
            <v-col>
                <v-subheader class="ml-8">Contato</v-subheader>
                <h1 class="ml-12 font-weight-bold display-2" id="font">Entre em contato</h1>
                <hr/>
            </v-col>
            <v-form >
                <v-row class="ml-12">
                    <v-col cols="12">
                        <v-text-field 
                            v-model="name"
                            label="Qual seu nome?"
                            required
                        ></v-text-field>
                    </v-col>
                    <v-col cols="12">
                        <v-text-field 
                            v-model="instituicao"
                            label="Qual sua instituição de ensino?"
                            required
                        ></v-text-field>
                    </v-col>
     
                    <v-col cols="12">
                        <v-text-field 
                            type="number"
                            v-model="periodo"
                            label="Qual seu período?"
                            required
                        ></v-text-field>
                    </v-col>
                    <v-btn color="green" depressed class="ma-2 white--text" @click="messageWhatsApp()">
                        Entrar em contato
                    </v-btn>
                </v-row>
            </v-form>
        </v-col>
        <v-col cols="4">
            <v-img
                :src="linkSrc"
                max-height="550"
                max-width="550"
            ></v-img>
        </v-col>
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
                const link = "https://api.whatsapp.com/send?phone=558188690954&text= *Olá, Glamour. Aqui é uma mensagem de teste* %0A %0A Meu nome é: *"+ this.name + "* %0A %0A Sou aluno da instituição: " + this.instituicao + "*, do " + this.periodo+"º período! ";
                window.open(link, "_blank")
                //alert("Vamos enviar para o zap")
            }

        }
    }   
</script>

<style scoped>

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
  margin-left: 50px !important;
  margin-top: 10px !important;
}

</style>