<template>
    <div>
        <div class="container mt-5">
            <h1 class="mt-5 text-center text-white bg-primary fst-italic rounded">PRODUCTOS</h1><br>
            <div class="row mt-3 g-5">
                <div class="col col-lg-4 col-md-6 col-sm-12 text-center" v-for="card in cards">
                    <div class="cards">
                        <div class="card" >
                            <img :src="card.image" :alt="card.mainTitle">
                                <div class="card-content">
                                    <h5>{{card.mainTitle}}</h5>
                                    <p>{{card.text}}</p>
                                    <div>
                                      <b-button variant="primary" @click="modalShow = !modalShow">Vista Previa</b-button>
                                        <b-modal v-model="modalShow">
                                          <div>
                                            <img :src="card.image" class="img-fluid" :alt="card.mainTitle">
                                          </div>
                                        </b-modal>
                                    </div>    
                                </div>
                        </div>
                    </div>
                </div>  
            </div>     
        </div>
    </div>
  </template>
  
  <script>
  export default {
  name: 'productos',
  data () {
    return {
      cards: [
        {
          image: require('@/assets/Aceites.jpg'),
          mainTitle: 'Aceites',
          text: 'Text1',
          index: 0
        },
        {
          image: require('@/assets/agua destilada.jpg'),
          mainTitle: 'Agua Destilada',
          text: 'Text2',
          index: 1
        },
        {
          image: require('@/assets/productos de limpieza.jpg'),
          mainTitle: 'Productos de Limpieza',
          text: 'Text3',
          index: 2
        },
        {
          image: require('@/assets/Gel de baño.jpg'),
          mainTitle: 'Gel de Baño',
          text: 'Text3',
          index: 3
        },
        {
          image: require('@/assets/Gel antibacterial.jpg'),
          mainTitle: 'Gel antibacterial',
          text: 'Text3',
          index: 4
        },
        {
          image: require('@/assets/Esencias.jpg'),
          mainTitle: 'Esencias',
          text: 'Text3',
          index: 5
        },
      ],
        modalShow: false
    }
  },
}
  </script>