<template>
  <div id="app">
    <b-navbar toggleable="lg" type="light" variant="light">
    <b-container>
      <b-navbar-brand href="#">
      <img src="@/assets/download.png" alt="logo">
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item to="/">HOME</b-nav-item>
        <b-nav-item to="about">NOSOTROS</b-nav-item>
        <b-nav-item to="productos">PRODUCTOS</b-nav-item>
      </b-navbar-nav>
      </b-collapse>
    </b-container>
      </b-navbar>
    <router-view/>  
    
    <div class="container-fluid p-3 bg-primary text-center text-white mt-5">
      <p >&copy; Todos los derechos reservados :: Proquimar :: Venezuela 2022 </p>
      <div class="container">
      <i class="fa-brands fa-instagram"> proquimar_ca</i><br>
      <i class="fa-brands fa-facebook"></i><br>
      <i class="fa-solid fa-phone"> (0295)263.2303/7150</i><br>
      <i class="fa-solid fa-mobile"> +58 412-0969723</i><br>
      <i class="fa-regular fa-envelope"></i><br>
      <i class="fa-solid fa-location-dot"> Av. 4 de Mayo, Minicentro Acuario, Local Nº. 5, 4 de Mayo, Porlamar, Margarita</i>
    </div>
    </div>
</div>


</template>
    

