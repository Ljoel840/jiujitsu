<template>
    <div class="container noticias">

        <!-- <h1 v-if="noti">NOTICIAS</h1>
        <div class="row alto" v-if="noti">
            <div class="col-md-4" v-for="not in noti" :key="not.id">
                <div class="row noticia">
                    <div class="contenedorTitulo"><h4 class="tituloNoticia"> {{not.titulo}} </h4> </div>
                    <img class="fotoNoticia" v-if="not.imagen.activo"  :src="not.imagen.url" alt="foto noticia">
                    <p class="textoNoticia" v-if="not.parrafos[0]">{{not.parrafos[0].texto}}</p>
                    <p class="textoNoticia" v-if="not.parrafos[1]">{{not.parrafos[1].texto}}</p>
                </div>
            </div>

        </div> -->
    
    <h1 v-if="noti">NOTICIAS</h1>
        <div class="row alto" v-if="noti">
            <div class="col-md-4" v-for="not in noti" :key="not.id">
                <div class="row noticia">
                    <div class="contenedorTitulo"><h4 class="tituloNoticia"> {{not.titulo}} </h4> </div>
                    <div class="contenido">
                        <video v-if="not.video.activo" width="90%" controls>
                             <source :src="not.video.url" type="video/mp4">
                                Your browser does not support HTML5 video.
                        </video>
                        <img class="fotoNoticia" v-if="not.imagen.activo && !not.boton.accion "  :src="not.imagen.url" alt="foto noticia">
                        <a v-if="not.boton.accion" :href="not.boton.accion" target="_blank">
                            <img class="fotoNoticia" v-if="not.imagen.activo"  :src="not.imagen.url" alt="foto noticia">
                        </a>
                        <p class="textoNoticia" v-if="not.parrafos[0]">{{not.parrafos[0].texto}}</p>
                        <p class="textoNoticia" v-if="not.parrafos[1]">{{not.parrafos[1].texto}}</p>
                    </div>
                </div>
            </div>

        </div>


    </div>
</template>

<script>
import axios from "axios";
export default {
    name: 'noticias',
    data () {
        return {
            noti:'',
            arregloOrdenado: []
        }
    },
    
    methods: {
  
        async obtenerDatos(){
            console.log(axios);
            let datos = await axios.post('https://apps.delfasoft.com/delfawebs/rest/dfs60024', {
                proyectoEnc: 'jiujitsu',
                pagina: '/'
            })
            .then (response=>{
                this.noti = response.data.frontBlogs;
                console.log(this.noti);
                this.arregloOrdenado = this.noti;
                this.arregloOrdenado.sort(function(a,b) {
                    return (b.orden - a.orden)
                })
                this.noti = this.arregloOrdenado;
                
            })
            .catch(error=>{
                console.log(error);
                this.noti = '';
                

            })
            
        },

        ordenarDatos(){
//             this.arregloOrdenado.sort(function (a, b){
//               return (b.orden - a.orden)
// })
        }
      
    },
    created(){
        this.obtenerDatos()
        this.ordenarDatos()
        
    }
}
</script>



<style scoped>
    .noticias {
        background-color: #fff;
    }
    h1 {
        text-align: center;
        padding: 2em 0 1em 0;
    }
    .noticia {
        width: 100%;
        background-color: #F4F0E5;
        border-radius: 10px;
        margin: 10px 0;
        justify-content: center;
        
    }
    .contenido {
        height:350px;
        text-align: center;
        overflow-y: auto;
    }
    .contenedorTitulo {
        border-radius: 10px 10px 0 0;
        background-color: #f58634;
        font-family: sans-serif;
        font-weight: bold;
        color: #000;
        text-align: center;
        width: 100%
    }

    .tituloNoticia {
        margin-top: 5px;
    }


    .fotoNoticia {
        width: 90%;
        margin-top: 10px;
        height: auto;
        text-align: center;

    }
    .textoNoticia {
        font-family: sans-serif;
        text-align: justify;
        line-height: 20px;
        padding: 10px;
        margin: 0;
    }
</style>