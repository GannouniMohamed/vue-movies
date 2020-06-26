<template>
 <div class="card">
   <img src="https://m.media-amazon.com/images/M/MV5BNDljZWNmYjItM2I2MC00MTkyLThhMmUtNGUwYzNhOGI4MGE2XkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg" alt="Avatar" style="width:100%">
   <div class="container">
     <h4><b>John Doe</b></h4> 
     <p>Architect & Engineer</p> 
   </div>
 </div>
</template>

<script>
export default {
  name: 'Card',
};
</script>

<style scoped>
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 40%;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

.container {
  padding: 2px 16px;
}
</style>