<template>
  <div>
      <article class="container">
            <div class="row">
                  <div class="col-md-6">
                      <img class="textoPrincipal" src="@/assets/img/t_jiujitsu.png" alt="Campeonato Panamericano de jiu jitsu">
                  </div>
                  <div class="col-md-6">
                      <img class="imagenPrincipal" src="@/assets/img/jiujitsu_atletas.png" alt="ATLETAS JIUJITSU">
                  </div>
            </div>
      </article>
      
      <poster/>
      <cronograma/>
      <noticias/>
      <enlaces/>
      <p_footer/>

  </div>


</template>

<script>
import p_footer from '@/components/p_footer.vue'
import poster from '@/components/poster.vue'
import cronograma from '@/components/cronograma.vue'
import noticias from '@/components/noticias.vue'
import enlaces from '@/components/enlaces.vue'
export default {
  name: 'home',
  components: {
    poster,
    cronograma,
    noticias,
    enlaces,
    p_footer
  }
}
</script>
<style scope>
    article {
        background-image: radial-gradient(#fdc579, #f58634);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        padding: 1em 0;
    }
    .textoPrincipal{
      width: 100%;
      padding: 3em;
       filter: drop-shadow(5px 15px 10px #B87C3B);
    }
     .imagenPrincipal{
      width: 100%;
      height: auto;
      padding: 1em;
    }
</style>
