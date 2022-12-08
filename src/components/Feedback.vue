<template>
    <v-col id="style-feedback">
        <template>
            <v-subheader class="ml-8">DEPOIMENTOS</v-subheader>
            <h1 class="ml-12 font-weight-bold display-2" id="font">Veja o que nossos clientes falam de nós!</h1>
            <hr/>
        </template>
        <v-row class="mt-2 mb-16">
          <v-card 
            v-for="item, index in items"
            :key="index"
            id="card01" 
            class="mx-auto mt-10 rounded-xl" 
            color="#34B450" 
            max-width="300" 
            max-height="300"
          >
            <v-list-item class="grow">

              <v-list-item-avatar color="grey darken-3" width="90" height="90">
                <v-img class="elevation-6"
                  :src="item.imgSrc"
                  :alt="item.nome"
                ></v-img >
              </v-list-item-avatar>

              <v-list-item-content>
                <v-list-item-title>{{item.nome}}</v-list-item-title>
                <v-list-item-title>{{item.instituicao}}</v-list-item-title>
              </v-list-item-content>  
            </v-list-item>

            <v-card-text 
              class="subtitle-1 text-justify" 
              id="text-card"
            >
              "{{item.relato}}"
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

              items:[
                {nome: "Priscila", instituicao: "Pedagogia, UFPE", relato: "Deu pra sentir toda atenção, carinho e responsabilidadee em cada detalhe. Ouvimos muitos elogios dos familiares e dos formandos também...", imgSrc: require('@/assets/feedback01.png')},

                {nome: "Letícia", instituicao: "Engenharia Civil, Unifavip", relato: "Gostaríamos de agradecer a vocês por tudo, pela organização de vocês, pelo cuidado com a gente e pela dedicação...", imgSrc: require('@/assets/feedback02.png')},

                {nome: "Tayná ", instituicao: "Fisioterapia, Univisa", relato: "...Fico imensamente feliz pelo resultado do trabalho maravilhoso de vocês. Desde o primeiro contato a todos os ajustes, não tinha dúvida que seria a empresa certa...", imgSrc: require('@/assets/feedback02.png')},
              ]

            }
        }
    }
    AOS.init();
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Fira+Sans+Condensed&display=swap');

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