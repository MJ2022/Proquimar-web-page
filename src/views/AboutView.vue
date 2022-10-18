<template>
  <div class="about">
    <b-container>
      <h1 class="mt-5 text-center text-white bg-primary fst-italic rounded"> NOSOTROS</h1><br>
      <p class="mt-5"> Somos una tienda fisica, con presencia desde 2000, dedicada a la comercialización de productos químicos en Venezuela</p>
    <b-row class="mt-5 mb-5">
    <b-col cols="12" md="8" lg="6">
      <p class="p-10 text-center h2 fst-italic"><u>Misión </u></p>
      <p class="text-justify">En La Tienda de Productos Químicos  estamos dedicados a la producción, almacenaje, venta y distribución de productos químicos con el fin de atender las demandas del sector  garantizando la seguridad y calidad. </p>
    </b-col>
    <b-col cols="12" md="4" lg="6">
      <p class="p-10 text-center h2 fst-italic"><u> Visión</u></p>
      <p class="text-justify">Trabajamos cada día para consolidar a Proquimar como la empresa de referencia para atender la demanda de productos químicos en toda Venezuela. Para ello ponemos todos nuestros esfuerzos  en garantizar la calidad y atención al cliente en todo el proceso de compra. </p>
    </b-col>
  </b-row>

  <div>
  <b-img center v-bind="mainProps" rounded src="@/assets/industria.jpg"  fluid alt="Responsive image" ></b-img>
</div>

    <b-row class="mt-5">
    <b-col>
      <p class="p-10 text-center h2 fst-italic"><u>Objetivo </u></p>
      <p class="text-justify">Atendemos  la demanda de aquellas empresas que buscan y necesitan materias primas para uso profesional o industrial, en procesos de producción o sin procesamiento alguno. Disponemos de un amplio catálogo y somos especialistas en la gestión de envases y embalajes para dar respuesta a las diferentes necesidades. </p>
    </b-col>
    </b-row>
  








  </b-container>
  </div>
</template>

<script>
  window.App = { host: '{{ url("/") }}/' }
</script>
