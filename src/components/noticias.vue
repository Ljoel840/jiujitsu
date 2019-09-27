<template>
    <div class="container noticias">
        <h1>NOTICIAS</h1>
        <div class="row">
            <div class="col-md-4" v-for="not in noti" :key="not.id">
                <div class="row noticia">
                    <div class="contenedorTitulo"><h4  class="tituloNoticia"> {{not.titulo}} </h4> </div>
                    <img class="fotoNoticia" :src="not.src" alt="foto noticia">
                    <p class="textoNoticia">{{not.noticia}}</p>
                    </div>
            </div>

        </div>




    </div>
</template>
<script>
export default {
    name: 'noticias',
    data () {
        return {
            noti : [
                {
                    titulo : 'Titulo Noticia 1',
                    src : require ('@/assets/img/foto_ejemplo.jpg'),
                    noticia : 'Lorem ipsum dolor sit amet consectetur adipiscing elit cras, volutpat dui eu integer sapien vivamus commodo, tortor faucibus nisl justo id praesent nisi nibh, mollis facilisis eget torquent nam taciti. Tincidunt lobortis morbi praesent ultrices scelerisque ac, pharetra aenean quam sociosqu fames condimentum, eget accumsan laoreet tristique parturient. Lobortis pellentesque odio justo fusce malesuada dapibus ridiculus a aptent risus, fames erat ullamcorper leo cum suspendisse placerat nam commodo morbi convallis, mollis blandit ultrices scelerisque rhoncus nascetur est molestie condimentum.'
                },
                {
                   titulo : 'Titulo Noticia 2',
                    src : require ('@/assets/img/foto_ejemplo.jpg'),
                    noticia : 'Lorem ipsum dolor sit amet consectetur adipiscing elit cras, volutpat dui eu integer sapien vivamus commodo, tortor faucibus nisl justo id praesent nisi nibh, mollis facilisis eget torquent nam taciti. Tincidunt lobortis morbi praesent ultrices scelerisque ac, pharetra aenean quam sociosqu fames condimentum, eget accumsan laoreet tristique parturient. Lobortis pellentesque odio justo fusce malesuada dapibus ridiculus a aptent risus, fames erat ullamcorper leo cum suspendisse placerat nam commodo morbi convallis, mollis blandit ultrices scelerisque rhoncus nascetur est molestie condimentum.'
                },
                {
                    titulo : 'Titulo Noticia 3',
                    src : require ('@/assets/img/foto_ejemplo.jpg'),
                    noticia : 'Lorem ipsum dolor sit amet consectetur adipiscing elit cras, volutpat dui eu integer sapien vivamus commodo, tortor faucibus nisl justo id praesent nisi nibh, mollis facilisis eget torquent nam taciti. Tincidunt lobortis morbi praesent ultrices scelerisque ac, pharetra aenean quam sociosqu fames condimentum, eget accumsan laoreet tristique parturient. Lobortis pellentesque odio justo fusce malesuada dapibus ridiculus a aptent risus, fames erat ullamcorper leo cum suspendisse placerat nam commodo morbi convallis, mollis blandit ultrices scelerisque rhoncus nascetur est molestie condimentum.'
                },
                {
                    titulo : 'Titulo Noticia 4',
                    src : require ('@/assets/img/foto_ejemplo.jpg'),
                    noticia : 'Lorem ipsum dolor sit amet consectetur adipiscing elit cras, volutpat dui eu integer sapien vivamus commodo, tortor faucibus nisl justo id praesent nisi nibh, mollis facilisis eget torquent nam taciti. Tincidunt lobortis morbi praesent ultrices scelerisque ac, pharetra aenean quam sociosqu fames condimentum, eget accumsan laoreet tristique parturient. Lobortis pellentesque odio justo fusce malesuada dapibus ridiculus a aptent risus, fames erat ullamcorper leo cum suspendisse placerat nam commodo morbi convallis, mollis blandit ultrices scelerisque rhoncus nascetur est molestie condimentum.'
                },



            ],
            conta:0,
           
        }
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