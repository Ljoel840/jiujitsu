<template>
    <div>
        <div class="container videos">
            <h1>TRANSMISION EN VIVO</h1>
            <iframe id="ls_embed_1570478096" src="https://livestream.com/accounts/12768295/events/8849008/player?width=640&height=360&enableInfoAndActivity=true&defaultDrawer=&autoPlay=true&mute=false" width="640" height="360" frameborder="0" scrolling="no" allowfullscreen> </iframe>
            
        </div>

    </div>
</template>

<script>
export default {
    name: 'p_video'
}
</script>

<style scoped>
    .videos {
        text-align: center;
        background-color: #fff;
        width: 100%;
        padding-bottom: 50px;
    }
    h1 {
            text-align: center;
            padding: 2em 0 1em 0;
        }
    #ls_embed_1570478096{
        width: 100%
    }
    
</style>