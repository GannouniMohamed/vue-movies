
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <carousel>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
    </carousel>
    <carousel>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
      <slide>
        <img width="50%" src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg">
      </slide>
    </carousel>
  </div>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel';

export default {
  name: 'hello',
  data() {
    return {
      msg: 'Welcome to Your Vue.js PWA from hello componenets',
    };
  },
  components: {
    Carousel,
    Slide,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #35495E;
}
</style>
