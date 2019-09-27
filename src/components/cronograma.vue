<template>
    <div class="flyers container">
        <div class="row p-0">
            <div class="col-md-6 pt-3">
                <h1 class="text-center">Cronograma</h1> 
                <div class="cronograma">
                    <h4>Jueves 10 de Octubre</h4>
                    <table width="100%">
                        <tr>
                            <td class="hora">09:00 a 17:00</td>
                            <td class="descripcion">Acreditación,entrega de uniformes (gi)</td>
                        </tr>
                        <tr>
                            <td class="hora">09:00 a 15:00</td>
                            <td class="descripcion">Cursos de arbitraje y actualización</td>
                        </tr>
                            <tr>
                            <td class="hora">17:00 a 18.00 </td>
                            <td class="descripcion">Pesaje extra oficial</td>
                        </tr>
                        <tr>
                            <td class="hora">18:00 a 20:00 </td>
                            <td class="descripcion">Pesaje Oficial atletas</td>
                        </tr>
                        <tr>
                            <td class="hora">20:30 a 22:30</td>
                            <td class="descripcion">Miting Tecnico (Sorteo de series)</td>
                        </tr>
                    </table>
                </div>
                 <div class="cronograma">
                    <h4>Viernes 11 de Octubre:</h4>
                    <table width="100%">
                        <tr>
                            <td class="hora">08:30 </td>
                            <td class="descripcion">Inicio de Competencias Duo U18,  Ne-Waza y Para JiuJitsu</td>
                        </tr>
                        <tr>
                            <td class="hora">10:30</td>
                            <td class="descripcion">Acto de inauguración</td>
                        </tr>
                            <tr>
                            <td class="hora">11:00 </td>
                            <td class="descripcion">Inicio de competencias</td>
                        </tr>
                        <tr>
                            <td class="hora">13:00  </td>
                            <td class="descripcion">Almuerzo</td>
                        </tr>
                        <tr>
                            <td class="hora">14:00 </td>
                            <td class="descripcion">Inicio de Competencias</td>
                        </tr>
                        <tr>
                            <td class="hora">18:00 </td>
                            <td class="descripcion">Inicio semifinales</td>
                        </tr>
                        <tr>
                            <td class="hora">18.00 a 20:00 </td>
                            <td class="descripcion">Pesaje Oficial atletas</td>
                        </tr>
                        <tr>
                            <td class="hora">19:30 </td>
                            <td class="descripcion">Fin de jornada y entrega de premiaciones</td>
                        </tr>
                    </table>
                </div>
                 <div class="cronograma">
                    <h4>Sábado 12 de Octubre:</h4>
                    <table width="100%">
                        <tr>
                            <td class="hora">08:30 </td>
                            <td class="descripcion">Inicio de Competencias Duo Adultos, Fighting U18, Mayores y Equipos</td>
                        </tr>
                        <tr>
                            <td class="hora">13:00 </td>
                            <td class="descripcion">Almuerzo</td>
                        </tr>
                            <tr>
                            <td class="hora">14:00 </td>
                            <td class="descripcion">Inicio de Competencias</td>
                        </tr>
                        <tr>
                            <td class="hora">18:00  </td>
                            <td class="descripcion">Inicio semifinales</td>
                        </tr>
                        <tr>
                            <td class="hora">19:30 </td>
                            <td class="descripcion">Fin de jornada y entrega de premiaciones</td>
                        </tr>
                    </table>
                </div>
                 <div class="cronograma">
                    <h4>Domingo 13 Octubre:</h4>
                    <table width="100%">
                        <tr>
                            <td class="hora">11.00 a 14.00 </td>
                            <td class="descripcion">Entrenamiento general</td>
                        </tr>
                    </table>
                </div>
                 <div class="cronograma">
                    <h4> Lunes 14 de Octubre:</h4>
                    <table width="100%">
                        <tr>
                            <td class="hora"></td>
                            <td class="descripcion">Salida de las delegaciones</td>
                        </tr>
                    </table>
                </div>
                <br>






            </div>
            <div class="col-md-6 flyer">
                <h1>Promoción Especial </h1> 
                <h1>Sólo para Atletas</h1>
                <img  class="imgFlyer" src="@/assets/img/flyer_promocion.jpg" alt="">
                <br>
            </div>
        </div>


    </div>
</template>
<script>
export default {
    name:'cronograma'
}
</script>

<style scoped>

    .flyers {
        background-color: #ECE4D9;
    }
    .flyer {
        width: 100%;
        padding: 1em;
        background-color: #f58634;
        text-align: center;
    }
    .flyer h1 {
        color: #ffffff;
        text-align: center;
    }

    tr:nth-child(odd) {
    background-color:#f2f2f2;
}


    .cronograma {
        width: 100%;
        background-color: #fff;
        margin-top: 10px;
        
    }
    .cronograma td {
        padding: 0 0 0 5px;
        font-family: sans-serif;

    }

    .cronograma h4 {
        color: #f58634;
        font-weight: bold;
        margin: 0;
        padding: 0 0 0 5px;
        /* font-size: 40px; */

    }


    .hora {
        width: 25%;
        
    }
    .descripcion {
       
        width: 100%;
    }


    .imgFlyer {
        margin-top: 20px;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        width: 80%;
       

    }
  

</style>