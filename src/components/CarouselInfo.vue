<template>
    <div class="events">
      <div class="container">
        <div class="card" @mouseover="preEvento = true" @mouseleave="preEvento = false">
            <h3 class="title">PRÉ EVENTO</h3>
            <div class="bar">
                <div class="emptybar">
                    <p>Pré evento é o primeiro evento oficial da turma. Realização de ensaios fotográficos para confecção dos materiais gráficos.</p>
                </div>
                <div class="filledbar"></div>
            </div>
        </div>
        <div class="card" @mouseover="aulaSaudade = true" @mouseleave="aulaSaudade = false">
            <h3 class="title">AULA DA <br> SAUDADE</h3>
            <div class="bar">
                <div class="emptybar">Concretiza-se a finalização de um ciclo. Momento no qual a turma recorda todos os milênios vividos juntos na instituição.</div>
                <div class="filledbar"></div>
            </div>
        </div>
        <div class="card" @mouseover="cultoEcumenico = true" @mouseleave="cultoEcumenico = false">
            <h3 class="title">CULTO ECUMÊNICO</h3>
            <div class="bar">
                <div class="emptybar">Cerimônia religiosa de formatura em que as pessoas refletem, agradecem e se conectam com sua fé.</div>
                <div class="filledbar"></div>
            </div>
        </div>
        <div class="card" @mouseover="colacaoDeGrau = true" @mouseleave="colacaoDeGrau = false">
            <h3 class="title">COLAÇÃO DE GRAU</h3>
            <div class="bar">
                <div class="emptybar">Cerimônia acadêmica tradicional e de caráter obrigatório para a outorga de grau do bacharel ou licenciado.</div>
                <div class="filledbar"></div>
            </div>
        </div>
        <div class="card" @mouseover="baileDeFormatura = true" @mouseleave="baileDeFormatura = false">
            <h3 class="title">BAILE DE FORMATURA</h3>
            <div class="bar">
                <div class="emptybar">O pré-evento é o momento em que a organização é efetivamente feita.</div>
                <div class="filledbar"></div>
            </div>
        </div>
        <div class="card" @mouseover="eventosCorporativos = true" @mouseleave="eventosCorporativos = false"> 
            <h3 class="title">EVENTOS CORPORATIVOS</h3>
            <div class="bar">
                <div class="emptybar">São uma das vias que nos proporcionam experiências e interações. Feiras, Workshops, confraternizações...</div>
                <div class="filledbar"></div>
            </div>
        </div>
      </div> 
      <div class="galeria">
        <div class="imagem-div">
          <div class="img-preEvento" v-if="preEvento">IMAGEM PRÉ EVENTO</div>
          <div class="img-aulaSaudade" v-if="aulaSaudade">IMAGEM AULA DA SAUDADE</div>
          <div class="img-cultoEcumenico" v-if="cultoEcumenico">IMAGEM CULTO ECUMENICO</div>
          <div class="img-colacaoGrau" v-if="colacaoDeGrau">IMAGEM COLAÇÃO DE GRAU</div>
          <div class="img-baileFormatura" v-if="baileDeFormatura">IMAGEM BAILE DE FORMATURA</div>
          <div class="img-eventosCorporativos" v-if="eventosCorporativos">IMAGEM EVENTOS CORPORATIVOS</div>
        </div>
        <div class="imagem-div">
          <div class="img-preEvento" v-if="preEvento">IMAGEM PRÉ EVENTO</div>
          <div class="img-aulaSaudade" v-if="aulaSaudade">IMAGEM AULA DA SAUDADE</div>
          <div class="img-cultoEcumenico" v-if="cultoEcumenico">IMAGEM CULTO ECUMENICO</div>
          <div class="img-colacaoGrau" v-if="colacaoDeGrau">IMAGEM COLAÇÃO DE GRAU</div>
          <div class="img-baileFormatura" v-if="baileDeFormatura">IMAGEM BAILE DE FORMATURA</div>
          <div class="img-eventosCorporativos" v-if="eventosCorporativos">IMAGEM EVENTOS CORPORATIVOS</div>
        </div>
        <div class="imagem-div">
          <div class="img-preEvento" v-if="preEvento">IMAGEM PRÉ EVENTO</div>
          <div class="img-aulaSaudade" v-if="aulaSaudade">IMAGEM AULA DA SAUDADE</div>
          <div class="img-cultoEcumenico" v-if="cultoEcumenico">IMAGEM CULTO ECUMENICO</div>
          <div class="img-colacaoGrau" v-if="colacaoDeGrau">IMAGEM COLAÇÃO DE GRAU</div>
          <div class="img-baileFormatura" v-if="baileDeFormatura">IMAGEM BAILE DE FORMATURA</div>
          <div class="img-eventosCorporativos" v-if="eventosCorporativos">IMAGEM EVENTOS CORPORATIVOS</div>
        </div>
        <div class="imagem-div">
          <div class="img-preEvento" v-if="preEvento">IMAGEM PRÉ EVENTO</div>
          <div class="img-aulaSaudade" v-if="aulaSaudade">IMAGEM AULA DA SAUDADE</div>
          <div class="img-cultoEcumenico" v-if="cultoEcumenico">IMAGEM CULTO ECUMENICO</div>
          <div class="img-colacaoGrau" v-if="colacaoDeGrau">IMAGEM COLAÇÃO DE GRAU</div>
          <div class="img-baileFormatura" v-if="baileDeFormatura">IMAGEM BAILE DE FORMATURA</div>
          <div class="img-eventosCorporativos" v-if="eventosCorporativos">IMAGEM EVENTOS CORPORATIVOS</div>
        </div>
      </div>
    </div>
</template>

<script>
    export default {
        name:"CarouselInfo",
        data(){
          return{
            preEvento: false,
            aulaSaudade: false,
            cultoEcumenico: false,
            colacaoDeGrau: false,
            baileDeFormatura: false,
            eventosCorporativos: false,
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

.galeria{
  display: grid;
  width: 50%;
  grid-template-columns: 300px 300px ;
}

.imagem-div{
  margin: 30px 0 30px 80px;
  background-color: blue;
  font-size: 15px;
  color: white;
  width: 250px;
  height: 250px;
}

.container {
  width: 50%;
  display: grid;
  grid-template-columns: 200px 200px 200px;
}

.card {
  display: flex;
  height: 280px;
  width: 200px;
  background-color: #34B450;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) -2px 3px 8px;
/*   margin-left: -50px; */
  transition: 0.4s ease-out;
  position: relative;
  left: 0px;
}

.card {
    margin-left: 80px;
}

.card:hover {
  transform: translateY(-20px);
  transition: 0.4s ease-out;
}

.title {
  color: white;
  font-weight: 300;
  position: absolute;
  left: 20px;
  top: 15px;
}

.bar {
  position: absolute;
  top: 100px;
  left: 20px;
  height: 5px;
  width: 150px;
}

.emptybar {
  background-color: #2e3033;
  width: 100%;
  height: 100%;

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

@media screen and (max-width: 900px){
  
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
    }

    
    .imagem-div{
      margin: 30px;
      background-color: blue;
     
    }

    .imagem-div div{
      width: 150px;
      height: 150px;
    }

    .events{
      margin: 0 auto;
      flex-direction: column;
    }
    
}

</style>