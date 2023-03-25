<template>
    <div class="events">
      <div class="container">
        <div class="card" v-for="(item, index) in items" :key="index" >
            <h3 class="title">{{ item.title }}</h3>
            <img src="https://www.pucgoias.edu.br/wp-content/uploads/2022/02/DSC_6379-1.jpg" alt="evento"/>
            <div class="bar">
                <div class="emptybar"> </div>
                <div class="filledbar"></div>
            </div>
            <p>{{ item.description }}</p>
        </div>
      </div> 
    </div>
</template>

<script>
    export default {
        name:"CarouselInfo",
        data(){
          return{
            items: [
              {title: "PRÉ EVENTO", description: "Pré evento é o primeiro evento oficial da turma. Realização de ensaios fotográficos para confecção dos materiais gráficos."},
              {title: "AULA DA SAUDADE", description: "Concretiza-se a finalização de um ciclo. Momento no qual a turma recorda todos os milênios vividos juntos na instituição."},
              {title: "CULTO ECUMÊNICO", description: "Cerimônia religiosa de formatura em que as pessoas refletem, agradecem e se conectam com sua fé."},
              {title: "COLAÇÃO DE GRAU", description: "Cerimônia acadêmica tradicional e de caráter obrigatório para a outorga de grau do bacharel ou licenciado."},
              {title: "BAILE DE FORMATURA", description: "O pré-evento é o momento em que a organização é efetivamente feita."},
              {title: "EVENTOS CORPORATIVOS", description: "São uma das vias que nos proporcionam experiências e interações. Feiras, Workshops, confraternizações..."},
            ]
          }
        }
    }
</script>

<style scoped>

.events{
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
    display: flex;
    flex-wrap: wrap;
    width: 80%;
    gap: 10px;
}

.card {
  display: flex;
  flex-direction: column;
  gap: 16px;
  height: 420px;
  width: 300px;
  background-color: #34B450;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) -2px 3px 8px;
  transition: 0.4s ease-out;
  position: relative;
  padding: 8px;
  margin-left: 80px;
}

.card p{
    text-align: justify;
}

.card img{
    border-radius: 8px;
}

.card:hover {
  transform: translateY(-20px);
  transition: 0.4s ease-out;
}

.title {
  color: white;
  font-weight: 300;
  top: 15px;
  width: 100%;
}

.bar {
  position: relative;
  height: 5px;
  width: 100%;
}

.emptybar {
  background-color: #125C07;
  width: 100%;
  height: 100%;
  border-radius: 8px;
}

.filledbar {
  position: absolute;
  top: 0px;
  z-index: 3;
  width: 0px;
  height: 100%;
  background: rgb(0,154,217);
  background: linear-gradient(90deg, rgba(0,154,217,1) 0%, rgba(217,147,0,1) 65%, rgba(255,186,0,1) 100%);
  transition: 0.6s ease-out;
}

.card:hover .filledbar {
  width: 120px;
  transition: 0.4s ease-out;
}

.card:hover .stroke {
  stroke-dashoffset: 100;
  transition: 0.6s ease-out;
}


@media screen and (max-width: 970px){
  
    .container{
        width: 100%;
        grid-template-columns: 200px 200px;
        gap: 20px;
    }
    .card:not(:first-child) {
      margin-left: 1px;
    }

    .card {
      margin-left: 0px;
    }

    .card:hover {
      transform: translateY(-20px);
      transition: 0.4s ease-out;
    }

    .card:hover ~ .card {
      position: relative;
      left: 0px;
      transition: 0.4s ease-out;
    }

    .galeria{
      width: 100%;
      display: grid;
      grid-template-columns: 200px 200px;
      gap: 20px;
    }
    
    .imagem-div{
      margin: 30px;
      background-color: blue;
    }

    .galeria div{
      width: 200px;
      padding: 10px;
      height: 200px;
      margin: 20px;
    }

    .events{
      margin: 0 auto;
      flex-direction: column;
    }
    
}

@media screen and (max-width: 400px){

    .galeria, .container{
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
    }
}

</style>