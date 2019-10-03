<template>
    <div id="app">
        <header class="container">
            <div class="row">
                <div class="col-md-6 izquierda">
                      <img class="logo" src="@/assets/img/logoCabecera.png" alt="instagram">
                </div>
                <div class="col-md-6 derecha">
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
            </div>
        </header>
        <div class="container p-0">
        <nav class="navbar navbar-expand-lg navbar-dark p-0">
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse flex-grow-0" id="navbarResponsive">
                  <ul class="navbar-nav">
                      <li class="nav-item">
                          <a class="nav-link" href="https://www.delfasport.com/#/">INICIO</a>
                      </li>
                      <li class="nav-item">
                          <router-link class="nav-link" to="/" exact>CAMPEONATO DE JIU-JITSU </router-link>
                      </li>
                  </ul>
            </div>
        </nav>
 



  
        </div>
    <router-view/>

    </div>

</template>

<style scoped>
    header {
        background-color: #fff;
        height: 80px;
        justify-content: flex-end;
        padding: 0 2em;
    }
    header a img {
        width: 30px;
        border: 5px;
        margin: 1.5em .5em;
    }

    .derecha {
      justify-items: right;
      text-align: right;
    }

    .isquierda {
      text-align: left;
    }

    .logo {
        height: 40px;
        border: 5px;
        margin: 1.5em .5em;
    }

    .navbar{
        color: #fff;
        
    }
    nav {
        background-color:  #34312c;
        display: flex;
        justify-content: center;
        color: #fff;
        font-family: sans-serif;
    }

    .navlink:hover{
        cursor:pointer;
        color: #000;
        background-color: white;
        
    }

    .router-link-active{
        background-color: #F58634; 
        font-weight: bold;
        
    }
    .navbar-toggler{
    color: #fff;
   
    }

 
   



    @media only screen and (min-width: 765px) {
    .derecha{
        display:inline;
    }
    

 }
 
 @media only screen and (max-width: 766px) {
    .derecha{
         display:none;
    }
    nav {
        justify-content: left;
      
    }

  }


</style>
