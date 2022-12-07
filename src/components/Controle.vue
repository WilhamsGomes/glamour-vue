<template>
    <div class="controle">
        <img id="app-cel" src="../assets/CELULAR2.png" alt="Aplicativo iFormando" width="850">
        <img id="maosCelularResp" src="../assets/mao&cll.png" alt="Aplicativo na tela do celular" width="350">
        <div class="maos">
            <img id="fraseControle" src="../assets/TEXTO.png" alt="Todo Controle em suas mãos">
            <img id="maosCelular" src="../assets/mao&cll.png" alt="Aplicativo na tela do celular" width="350">
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

@media screen and (max-width: 800px) {

    .controle{
        background-color: #34B450;
        display:flex;
        flex-direction: column-reverse;
        align-items: center;
        justify-content: center;
    }

    #maosCelular{
        display: none;
    }

    .maos{
        display:flex;
        align-items: center;
        margin-left: 0px;
        margin-top: 180px;
    }

    .controle img{
        margin-top: -150px;
    }

    .controle img{
       width: 100%;
    }

    img{
        width: 150px;
    }

    #maosCelularResp{
        display:none;
    }

}

@media screen and (max-width: 1400px) {

    #maosCelular{
        display: none;
    }
}


@media screen and (max-width: 1100px) and (min-width: 799px){

    .controle{
        display:flex;
        flex-direction: column-reverse;
        align-items: center;
        justify-content: center;
    }

    .controle img{
        margin-left: -200px;
    }

    .maos{
        margin-top: 0px;
    }


    #fraseControle{
        margin: 0 auto;
    }

    #maosCelularResp{
        margin-top: 330px;
        margin-left: 450px;
        position: absolute;
        display: block;
    }

}

@media screen and (max-width: 840px){
    #maosCelularResp{
        display:none;
    }
}

</style>