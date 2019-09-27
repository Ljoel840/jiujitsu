<template>
    <div class="posters container">
        <div class="row p-0">
            <div class="col-md-6 poster">
                <img  class="imgPoster" id="myImg" src="@/assets/img/poster_jiujitsu.jpg" alt="Poster Jiu-Jitsu">
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
        <div id="myModal" class="modal">
            <span class="close">&times;</span>
            <img class="modal-content" id="img01">
            <div id="caption"></div>
        </div>
        <br>

    </div>
</template>
<script>
export default {
    name:'poster',
    mounted () {
            // Get the modal
            var modal = document.getElementById("myModal");

            // Get the image and insert it inside the modal - use its "alt" text as a caption
            var img = document.getElementById("myImg");
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

/* --------------------------- */

#myImg {
  cursor: pointer;
  transition: 0.3s;
}

#myImg:hover {opacity: 0.7;}

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