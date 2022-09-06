<template>
 <v-app id="inspire">
    <NavBar/>
    <PageInicial/>
    <Numbers/>
    <Feedback/>
    <Carrossel/>
    <Controle/>
    <CarouselInfo/>
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
    Video
}
    }
</script>

<style scoped>

  #inspire{
    background-color: #fff;
  }
  
  .img-flutuante{
      position: absolute;
      width: 180px;
      left: 40px;
      top: 80px;
      animation: rotate 5s linear infinite;
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
