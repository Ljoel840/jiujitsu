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
                <img  class="imgFlyer" id="myImg2" src="@/assets/img/flyer_promocion.jpg" alt="Flyer Jiu-jitsu" >
                <br>
            </div>
            <div id="myModal" class="modal">
                <span class="close">&times;</span>
                <img class="modal-content" id="img01">
                <div id="caption"></div>
            </div>
        </div>


    </div>
</template>
<script>
export default {
    name:'cronograma',
    mounted() {
            // Get the modal
            var modal = document.getElementById("myModal");

            // Get the image and insert it inside the modal - use its "alt" text as a caption
            var img = document.getElementById("myImg2");
            var modalImg = document.getElementById("img01");
            var captionText = document.getElementById("caption");
            img.onclick = function(){
            modal.style.display = "block";
            modalImg.src = this.src;
            captionText.innerHTML = this.alt;
            }

            // Get the <span> element that closes the modal
            var span = document.getElementsByClassName("close")[0];

            // When the user clicks on <span> (x), close the modal
            span.onclick = function() { 
            modal.style.display = "none";
            }



    }
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
  

/* --------------------------- */

#myImg2 {
  cursor: pointer;
  transition: 0.3s;
}

#myImg2:hover {opacity: 0.7;}

/* The Modal (background) */
.modal {
  display: none; /* Hidden by default */
  position: fixed; /* Stay in place */
  z-index: 1; /* Sit on top */
  padding-top: 100px; /* Location of the box */
  left: 0;
  top: 0;
  width: 100%; /* Full width */
  height: 100%; /* Full height */
  overflow: auto; /* Enable scroll if needed */
  background-color: rgb(0,0,0); /* Fallback color */
  background-color: rgba(0,0,0,0.9); /* Black w/ opacity */
}

/* Modal Content (image) */
.modal-content {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
}

/* Caption of Modal Image */
#caption {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
  text-align: center;
  color: #ccc;
  padding: 10px 0;
  height: 150px;
}

/* Add Animation */
.modal-content, #caption {  
  -webkit-animation-name: zoom;
  -webkit-animation-duration: 0.6s;
  animation-name: zoom;
  animation-duration: 0.6s;
}

@-webkit-keyframes zoom {
  from {-webkit-transform:scale(0)} 
  to {-webkit-transform:scale(1)}
}

@keyframes zoom {
  from {transform:scale(0)} 
  to {transform:scale(1)}
}

/* The Close Button */
.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  transition: 0.3s;
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}

/* 100% Image Width on Smaller Screens */
@media only screen and (max-width: 700px){
  .modal-content {
    width: 100%;
  }
}







</style>