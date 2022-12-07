<template>
    <div class="text-center">
      <v-menu>
            <template v-slot:activator="{ on: menu, attrs }">
                <v-tooltip bottom>
                    <template v-slot:activator="{ on: tooltip }">
                        <v-avatar >
                            <v-icon 
                                color="#fff" 
                                class="mx-2"
                                v-bind="attrs"
                                v-on="{ ...tooltip, ...menu }"
                            >mdi-menu
                            </v-icon>
                        </v-avatar>
                    </template>
                    <span>Clique para abrir o menu</span>
                </v-tooltip>
            </template>
            <v-list color="#125C07" dark>
                <v-list-item
                    v-for="(item, index) in items"
                    :key="index"
                    class="item-list"
                >
                    <v-list-item-title>{{ item.title }}</v-list-item-title>
                </v-list-item>
            </v-list>
      </v-menu>
    </div>
</template>

<script>

    export default{
        name:"NavBarResponsivo",
        data: () => ({
            items: [
                { title: 'Home' },
                { title: 'Eventos' },
                { title: 'Serviços' },
                { title: 'Contato' },
            ],
        }),
    }

</script>

<style scoped>

.item-list:hover{
    cursor: pointer;
    background-color: #2c861e;
    transition: 1.5s;
}

</style>