<template>
    <v-container fluid>
      <v-row>
        <v-col cols="12" sm="12" md="6" offset-md="3" >
          <v-card>
              <v-fab-transition>
                <v-btn class="mt-16"
                  color="green"
                  dark
                  fixed
                  bottom
                  right
                  fab
                >
                  <v-icon>mdi-account-heart</v-icon>
                </v-btn>
              </v-fab-transition>

          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </template>

<script>
    export default {
        name:"BtnWhatsApp",
        data: () => ({
            hidden: false,
        }),
    }
</script>

<style scoped>

</style>