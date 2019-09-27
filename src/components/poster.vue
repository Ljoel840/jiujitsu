<template>
    <div class="posters container">
        <div class="row p-0">
            <div class="col-md-6 poster">
                <img  class="imgPoster" src="@/assets/img/poster_jiujitsu.jpg" alt="">
            </div>
            <div class="col-md-6 pt-3">
                <div class="row textoCampeonato">
                    <h4>GRAN CAMPEONATO PANAMERICANO DE JIU-JITSU </h4>
                    <h4>EN URUGUAY</h4>
                    <h4>DESDE EL CAMPUS DE MALDONADO </h4>
                    <h4>ESTE MES DE OCTUBRE </h4>
                    <h3>TE ESPERAMOS</h3>
                    <h4>VIERNES 11 y SABADO 12 </h4>
                    <h4>GRAN NIVEL DE COMPETIDORES</h4>
                    <br>
                    <h4>ORGANIZA: </h4>
                    <h4>PTE DE FEDERACION DE JIU JITSU</h4>
                    <h4>Gregory Vallarino </h4>
                    <h4> Peace and Sport</h4>
                </div>
                <div class="row logosPatrocinadores">
                    <img class="logos" src="@/assets/img/l_fujj.png" alt="">
                    <img class="logos" src="@/assets/img/l_panamerican.png" alt="">
                    <img class="logos" src="@/assets/img/l_federacion.png" alt="">
                    <img class="logos" src="@/assets/img/l_maldonado.png" alt="">
                    <img class="logos" src="@/assets/img/l_secretaria.png" alt="">
                    <img class="logos" src="@/assets/img/l_mevuelo.png" alt="">
                    <img class="logos" src="@/assets/img/l_improveit.png" alt="">
                    <img class="logos2" src="@/assets/img/l_delfasport.png" alt="">

                </div>

            </div>
        </div>
        <br>

    </div>
</template>
<script>
export default {
    name:'poster'
}
</script>

<style scoped>

    .posters {
        background-color: #fff;
    }
    .poster {
        width: 100%;
        padding: 1em;
        text-align: center;
    }

    .imgPoster {
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        width: 90%;
        margin-top: 2em;

    }
    .textoCampeonato {
        padding: 1em;
        margin: 0;
        text-align: center;
        justify-content: center;
        display: inline;
        
    }

    .textoCampeonato h4 {
        font-weight: bold;
        font-size: 20px;
        text-align: center;
        padding: 0;
        line-height: 20px;
        margin-bottom: 10px;
        
    }

    .textoCampeonato h3 {
        color: #f58634;
        font-weight: bold;
        font-size: 40px;

    }
    .logos {
        height: 80px;
        width: auto;
        margin: 10px;
    }
    .logos2 {
        height: 40px;
        width: auto;
        margin: 10px;
    }
    .logosPatrocinadores {
        align-content: space-around;
        justify-content: center;
        align-items: center;
    }

</style>