<template>
    <v-footer dark padless >
      <v-card class="flex" flat tile >
        <!-- <v-card-title class="green">
          <strong class="subheading">Get connected with us on social networks!</strong>
  
          <v-spacer></v-spacer>
  
          <v-btn v-for="icon in icons" :key="icon" class="mx-4" dark icon >
            <v-icon size="24px">
              {{ icon }}
            </v-icon>
          </v-btn>
        </v-card-title>-->
  
        <v-card-text class="py-2 white--text text-center">
          {{ new Date().getFullYear() }} — <strong> Glamour Assessoria de Eventos &#169 Todos os direitos reservados</strong>
        </v-card-text>
      </v-card>
    </v-footer>
</template>

<script>
    export default {
        name:"Footer",
        data: () => ({
            icons: [
                'mdi-facebook',
                'mdi-twitter',
                'mdi-linkedin',
                'mdi-instagram',
            ],
        }),
    }
</script>

<style>

</style>