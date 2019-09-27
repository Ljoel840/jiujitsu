<template>
    <div class="container enlaces">
        <h1>ENLACES DE INTERES</h1>
        <div class="row">
            <div class="col-md-3 p-4 enlace">
                <a href="https://www.facebook.com/Campeonato-Panamericano-de-JiuJitsu-Uruguay-2019-111122373569234/" target="_blank" rel="noopener noreferrer">
                    <img  class="imgEnlaces" src="@/assets/img/enlace1.png" alt="Facebook Campeonato Jiu-Jitsu">
                    <p class="textoEnlaces">Facebook Oficial del Campeonato</p>
                </a>
            </div>
            <div class="col-md-3 p-4 enlace">
                <a href="http://fujj.com.uy/jiujitsu-japones/" target="_blank" rel="noopener noreferrer">
                    <img  class="imgEnlaces" src="@/assets/img/enlace2.png" alt="Web Federacion Jiu-jitsu">
                    <p class="textoEnlaces">Información Jiu-Jitsu</p>
                </a>
            </div>
            <div class="col-md-3 p-4 enlace">
                <a href="https://www.facebook.com/JuJitsuworldfightingduonewaza/" target="_blank" rel="noopener noreferrer">
                    <img  class="imgEnlaces" src="@/assets/img/enlace3.png" alt="Facebook NFull Ippon Magazine">
                    <p class="textoEnlaces">Full Ippon Magazine</p>
                </a>
            </div>
            <div class="col-md-3 p-4 enlace">
                <a href="https://www.facebook.com/jiujitsumx/" target="_blank" rel="noopener noreferrer">
                    <img  class="imgEnlaces" src="@/assets/img/enlace4.png" alt="Facebook Seleccion Mexicana de Jiu-Jitsu">
                    <p class="textoEnlaces">Selección Mexicana de Jiu-Jitsu</p>
                </a>
            </div>
        </div>
        <br>



    </div>
</template>
<script>
export default {
    name: 'enlaces'
}
</script>



<style scoped>
    .enlaces {
        background-color: #fff;
        padding: 0;
    }
    h1 {
        text-align: center;
        padding: 2em 0 1em 0;
    }
 
    .row {
        background-color: #B5A897;
        margin: 0;
        text-align: center;
    }

    .imgEnlaces {
        width: 70%;
        padding: 10px;
    }
    .textoEnlaces{
        font-family: sans-serif;
        color:#fff;
        text-decoration: none;
    }

    .enlace:hover {
        filter: drop-shadow(0px 0px 10px #B87C3B);
    }
    
</style>