<template>
    <div class="controle">
        <img src="../assets/CELULAR2.png" alt="Aplicativo iFormando" width="850">
        <div class="maos">
            <img src="../assets/TEXTO.png" alt="Todo Controle em suas mãos">
            <img src="../assets/mao&cll.png" alt="Aplicativo na tela do celular" width="350">
        </div>
    </div>
</template>

<script>
    export default {
        name:"Controle"
    }
</script>

<style scoped>

.controle{
    background-color: #34B450;
    display:flex;
    align-items: center;
    justify-content: space-between;
}

.controle img{
    margin-top: -150px;
}

.maos{
    display:flex;
    align-items: center;
    margin-left: -280px;
    margin-top: 180px;
}


</style>