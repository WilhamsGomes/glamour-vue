<template>
 <v-app id="inspire">
    <NavBar/>
    <PageInicial/>
 
    <img id="logoG" src="../assets/LOGO.G-VERDE.png"/>
    <Numbers/>
    <CarouselInfo/>
    <Feedback/>
    <Controle/>
    
    <FlipbookPhoto/>
    <FormWhatsApp/>
    <Video/>
    <Footer/>
  </v-app>
</template> 

<script>

  import NavBar from "@/components/NavBar.vue";
  import Numbers from "@/components/Numbers.vue";
  import PageInicial from "@/components/PageInicial.vue";
  import Feedback from "@/components/Feedback.vue";
  import Carrossel from "@/components/Carrossel.vue";
  import Controle from "@/components/Controle.vue";
  import CarouselInfo from "@/components/CarouselInfo.vue";
  import Footer from "@/components/Footer.vue";
  import Video from "@/components/Video.vue";
  //import BtnWhatsApp from "@/components/BtnWhatsApp.vue";
  import FlipbookPhoto from "@/components/FlipbookPhoto.vue";
  import FormWhatsApp from "@/components/FormWhatsApp.vue";
  
    export default {
      name:"HomeView",

      data: () => ({
          links: [
              "Dashboard",
              "Messages",
              "Profile",
              "Updates",
          ],
      }),
      components: {
        NavBar,
        Numbers,
        PageInicial,
        Feedback,
        Carrossel,
        Controle,
        CarouselInfo,
        Footer,
        Video,
      // BtnWhatsApp,
        FlipbookPhoto,
        FormWhatsApp
      }
    }
</script>

<style scoped>

  #inspire{
    background-color: #fff;
  }
  
  #logoG{
    margin-top: 60px;
    left: 60%;
    width: 600px;
    z-index: 20;
    position: absolute;
    opacity: 1;
  }
  
  @keyframes rotate {
      0%{
         top: 80px;
      }
  
      25%{
          top: 120px;
      }
  
      50%{
          top: 160px;
      }
  
      75%{
          top: 140px;
      }
  
      100%{
          top: 120px;
      }
  }
  
  </style>
