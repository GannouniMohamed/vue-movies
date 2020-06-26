
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <carousel :autoplay="true" :navigationEnabled="true">
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
    </carousel>
    <carousel>
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
      <slide>
        <card />
      </slide>
    </carousel>
  </div>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel';
import Card from './Card';

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
    Card,
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
