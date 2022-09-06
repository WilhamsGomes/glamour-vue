<template>
    <v-row class="mt-16 mb-16">

      <v-card id="card01" class="mx-auto mt-10 rounded-xl" color="#34B450" dark max-width="400" >
      
        <v-card-actions>
        <v-list-item class="grow">
          <v-list-item-avatar color="grey darken-3">
            <v-img class="elevation-6" alt=""
              src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
            ></v-img>
          </v-list-item-avatar>

          <v-list-item-content>
            <v-list-item-title>Priscila Sobrenome</v-list-item-title>
            <v-list-item-title>Pedagogia, UFPE</v-list-item-title>
          </v-list-item-content>  
        </v-list-item>
      </v-card-actions>

      <v-card-text class="text-h5 font-weight-bold">
        "Deu pra sentir toda atenção, carinho e responsabilidadee em cada detalhe. Ouvimos muitos elogios dos familiares e dos formandos também..."
      </v-card-text>

      </v-card> 

      <v-card id="card01" class="mx-auto mt-10 rounded-xl" color="#34B450" dark max-width="400" >
      
      <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img class="elevation-6" alt=""
            src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>Evan You</v-list-item-title>
          <v-list-item-title>Curso</v-list-item-title>
        </v-list-item-content>  
      </v-list-item>
    </v-card-actions>

    <v-card-text class="text-h5 font-weight-bold">
      "Deu pra sentir toda atenção, carinho e responsabilidadee em cada detalhe. Ouvimos muitos elogios dos familiares e dos formandos também..."
    </v-card-text>

      </v-card> 

      <v-card id="card01" class="mx-auto mt-10 rounded-xl" color="#34B450" dark max-width="400" >
      
      <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img class="elevation-6" alt=""
            src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>Evan You</v-list-item-title>
          <v-list-item-title>Curso</v-list-item-title>
        </v-list-item-content>  
      </v-list-item>
    </v-card-actions>

    <v-card-text class="text-h5 font-weight-bold">
      "Deu pra sentir toda atenção, carinho e responsabilidadee em cada detalhe. Ouvimos muitos elogios dos familiares e dos formandos também..."
    </v-card-text>

      </v-card> 

    </v-row>
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

#card01::before{
    font-family: 'Roboto' !important;
    content: ' " ';
    position: absolute;
    font-size: 185px;

    color: #125C07;
    top: -50px;
    left: 80%;
    opacity: 0.4;
} 

</style>