<template>
   
    <footer class="container p-0 ">
        <div class="row p-0 m-0 foot">
            <div class="p-2">
                    <a href="http://www.Instagram.com/delfasport" target="_blank" rel="noopener noreferrer">
                        <img src="@/assets/img/h_instagram.png" alt="instagram">
                    </a>
                    <a href="http://www.facebook.com/delfasport" target="_blank" rel="noopener noreferrer">
                        <img src="@/assets/img/h_facebook.png" alt="facebook">
                    </a>                            
                    <a href="http://twitter.com/delfasport" target="_blank" rel="noopener noreferrer">
                        <img src="@/assets/img/h_twitter.png" alt="twitter">
                    </a>                            
                    <a href="http://youtube.com/delfasoft" target="_blank" rel="noopener noreferrer">
                        <img src="@/assets/img/h_youtube.png" alt="youtube">
                    </a>
            </div>
            <div class="p-2" >
                    <img src="@/assets/img/logoCabecera.png" alt="Logo de delfasport" class="logo">
            </div>
        </div>
        <div class="row pie p-0 m-0">
            <a href="https://delfasoft.com" target="_blank" class="pie d-flex justify-content-between" rel="noopener noreferrer">
                <span>delfasoft © 2019</span>
                <span>versión 0.1.0</span>
             </a>
        </div>
    </footer>
</template>
<script>
export default {
    name: 'p_footer'
}
</script>

<style scoped>
    footer {
        width: 100%;
        background-color: #34312c;
        height: auto;
        /* justify-content: flex-end; */
        /* padding: 0 2em; */
        
    }
    footer a img {
        width: 50px;
        border: 5px;
        margin: 1.5em .5em;
    }


    div a:focus img {
        border-radius: 5px;
        box-shadow: 0 0 1em #f58634;
    }

    .iconos {
       justify-content: space-between
    }

    .foot {
        padding: 0;
        justify-content: space-between;
        text-align: center;
    }

    .logo {
        margin: 2em .5em 2em auto;
    }

    .pie {
        width: 100%;
        margin: 0;
        background-color: #292929;
        justify-content: space-between;
        padding: 0;
    }

    .pie:focus {
        background-color: #524f50;
    }

    span {
        color: #fff;
        padding: 1em;
    }

</style>
