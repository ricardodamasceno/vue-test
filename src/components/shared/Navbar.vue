<template>
  <div id="histNavbar">
    <nav class="navbar navbar-toggleable-md navbar-light navbar-dark bg-faded">
      <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse"
              data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
              aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <a class="navbar-brand green-text ml-5" routerLink="/home" routerLinkActive="active">Historiador Digital</a>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto pr-5 ">
          <li class="nav-item p-1">
            <a id="home-menu-item" routerLink="/home" routerLinkActive="active" class="nav-link menu-link white-text "
               href="#">Home <span class="sr-only">(current)</span></a>
          </li>
          <li class="nav-item p-1">
            <a id="historia-brasil-menu-item" routerLink="/post-1" routerLinkActive="active"
               class="nav-link menu-link white-text" href="#">História
              do Brasil</a>
          </li>
          <li class="nav-item p-1">
            <a id="historia-internacional-menu-item" routerLink="/post-1" routerLinkActive="active"
               class="nav-link menu-link white-text" href="#">História Internacional</a>
          </li>
        </ul>
        <form class="form-inline my-2 my-lg-0 mr-5">
          <input class="form-control mr-sm-2" type="text" placeholder="Pesquisar post ...">
          <button class="btn btn-outline-success search-button my-2 my-sm-0 green-text" type="submit">Pesquisar</button>
        </form>
      </div>
    </nav>
  </div>
</template>

<script>



export default {
  created () {
    $('#home-menu-item').addClass('colored-green-border')
  }
}
</script>

<style>
  .navbar-dark {
    background-color: #1d1e1f;
  }

  .search-button:hover {
    color: #1d1e1f !important;
    cursor: pointer;
  }

  .menu-link:hover {
    transition-property: border-color !important;
    transition-duration: 0.5s !important;
    transition-timing-function: linear;
    transition-timing-function: cubic-bezier(0.005, 0.625, 0.365, 0.0840);
    border-bottom: solid 3px darkgreen !important;
  }

  .colored-green-border {
    border-bottom: solid #44ee99;
  }
</style>
