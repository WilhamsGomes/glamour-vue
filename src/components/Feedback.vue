<template>
    <v-col id="style-feedback">
        <template >
            <v-subheader class="ml-8">DEPOIMENTOS</v-subheader>
            <h1 class="ml-12 font-weight-bold display-2" id="font">Veja o que nossos clientes falam de nós!</h1>
            <hr/>
        </template>
        <v-row class="mt-2 mb-16">
          <v-card id="card01" class="mx-auto mt-10 rounded-xl" color="#34B450" max-width="300" max-height="300">
            <v-card-actions>
            <v-list-item class="grow">
              <v-list-item-avatar color="grey darken-3" width="90" height="90">
                <v-img class="elevation-6" alt=""
                  src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
                ></v-img >
              </v-list-item-avatar>

              <v-list-item-content>
                <v-list-item-title>Priscila Sobrenome</v-list-item-title>
                <v-list-item-title>Pedagogia, UFPE</v-list-item-title>
              </v-list-item-content>  
            </v-list-item>
          </v-card-actions>

          <v-card-text class="subtitle-1 text-justify" id="text-card">
            "Deu pra sentir toda atenção, carinho e responsabilidadee em cada detalhe. Ouvimos muitos elogios dos familiares e dos formandos também..."
          </v-card-text>

          </v-card> 

          <v-card id="card01" class="mx-auto mt-10 rounded-xl" color="#34B450" max-width="300" max-height="300">
            <v-card-actions>
            <v-list-item class="grow">
              <v-list-item-avatar color="grey darken-3" width="90" height="90">
                <v-img class="elevation-6" alt=""
                  src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
                ></v-img >
              </v-list-item-avatar>

              <v-list-item-content>
                <v-list-item-title>Priscila Sobrenome</v-list-item-title>
                <v-list-item-title>Pedagogia, UFPE</v-list-item-title>
              </v-list-item-content>  
            </v-list-item>
          </v-card-actions>

          <v-card-text class="subtitle-1 text-justify" id="text-card">
            "Deu pra sentir toda atenção, carinho e responsabilidadee em cada detalhe. Ouvimos muitos elogios dos familiares e dos formandos também..."
          </v-card-text>

          </v-card> 
          
          <v-card id="card01" class="mx-auto mt-10 rounded-xl" color="#34B450" max-width="300" max-height="300">
            <v-card-actions>
            <v-list-item class="grow">
              <v-list-item-avatar color="grey darken-3" width="90" height="90">
                <v-img class="elevation-6" alt=""
                  src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
                ></v-img >
              </v-list-item-avatar>

              <v-list-item-content>
                <v-list-item-title>Priscila Sobrenome</v-list-item-title>
                <v-list-item-title>Pedagogia, UFPE</v-list-item-title>
              </v-list-item-content>  
            </v-list-item>
          </v-card-actions>

          <v-card-text class="subtitle-1 text-justify" id="text-card">
            "Deu pra sentir toda atenção, carinho e responsabilidadee em cada detalhe. Ouvimos muitos elogios dos familiares e dos formandos também..."
          </v-card-text>

          </v-card> 
        </v-row>
    </v-col>
</template>

<script>
    import AOS from 'aos';
    import 'aos/dist/aos.css'; 

    export default {
        name: "Feedback",
        data(){
            return{

            }
        }
    }
    AOS.init();
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Fira+Sans+Condensed&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Crete+Round&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Cantata+One&display=swap');

#font{
  font-family: 'Fira Sans Condensed' !important;
}

#text-card{
  color: white !important;
}

#card01:hover{
    transition: 0.75s ease-in-out;
}

#card01:hover{
    transform: scale(1.02);
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