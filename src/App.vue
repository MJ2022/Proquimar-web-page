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
        <b-nav-item to="/">Home</b-nav-item>
        <b-nav-item to="about">Nosotros</b-nav-item>
        <b-nav-item to="productos">Productos</b-nav-item>
      </b-navbar-nav>
      </b-collapse>
    </b-container>
      </b-navbar>
    <router-view/>
</div>
    

