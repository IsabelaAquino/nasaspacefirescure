<template>
        <nav class="navbar navbar-expand-lg navbar-light fixed-top py-3" id="mainNav">
          <div class="container">
            <img style="width: 180px;" src="../../img/logo.jpg" alt="logo da fire">
            <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarResponsive">
              <ul class="navbar-nav ml-auto my-2 my-lg-0">
                <li class="nav-item">
                  <a class="nav-link js-scroll-trigger" href="#about">Home</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link js-scroll-trigger" href="#services">Reportar</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link js-scroll-trigger" href="#portfolio">Linha do tempo</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link js-scroll-trigger" href="#contact">Relatóros</a>
                </li>
              </ul>
            </div>
          </div>
        </nav>
</template>
<script>
export default {
    data(){
        return {

        }
    },
    methods:{

    }
}
</script>
<style scoped>
.navbar{
  display: block;
  background-color: rgb(255, 141, 2);
}
.nav-link{
  color: azure !important;
}
</style>