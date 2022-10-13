<template>
  <div class="home">
    <b-container>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="5000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
  
      <b-carousel-slide
        caption="Productos Quimicos"
        text="Todo lo que necesitas para la limpieza y mucho mas !!!"
        img-src= "proquimar/src/assets/slide-1.png"
      ></b-carousel-slide>

      <b-carousel-slide img-src="proquimar/src/assets/slide-2.png">
        <h1>Maxima Calidad y Respeto al Medio Ambiente</h1>
      </b-carousel-slide>

      <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=58"></b-carousel-slide>
      </b-carousel>
    </b-container>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
  }
</script>

 

