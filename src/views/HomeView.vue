<template>
  <div class="home">
    <b-container>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#fff"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
  
      <b-carousel-slide
        caption="Productos Quimicos"
        text="Todo lo que necesitas para la limpieza y mucho mas !!!"
        img-src= "@/assets/slide1.jpg"
      ></b-carousel-slide>

      <b-carousel-slide img-src="@/assets/slide-2.jpg">
        <h1>Maxima Calidad y Respeto al Medio Ambiente</h1>
      </b-carousel-slide>

      <b-carousel-slide img-src="@/assets/slide-3.jpg">
      <h1>Productos en venta al detal y al mayor</h1>
    </b-carousel-slide>
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

 

