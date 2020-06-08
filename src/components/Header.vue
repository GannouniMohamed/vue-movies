<template>
  <header>
    <ul class="sidenav">
      <li><a class="active" href="/home"> <font-awesome-icon icon="home" /> HOME </a></li>
      <li><a href="/movies"> <font-awesome-icon icon="film" /> MOVIES </a></li>
      <li><a href="/series"> <font-awesome-icon icon="tv" /> SERIES </a></li>
    </ul>
  </header>
</template>

<script>
export default {
  name: 'Header',
};
</script>

<style scoped>
header {
  margin: 0;
  height: 56px;
  padding: 0 16px 0 24px;
  color: #ffffff;
  display: flex;
  justify-content: center;
  align-items: center;
}

  ul.sidenav {
    list-style-type: none;
    margin: 0;
    padding: 0;
    position: fixed;
    overflow: auto;
    margin: auto;
  }

  ul.sidenav li a {
    display: block;
    color: #000;
    padding: 8px 16px;
    text-decoration: none;
  }
  
  ul.sidenav li a.active {
    background-color: #4CAF50;
    color: white;
  }

  ul.sidenav li a:hover:not(.active) {
    background-color: #555;
    color: white;
  }

  @media screen and (max-width: 900px) {
    ul.sidenav {
      height: auto;
      position: relative;
    }
    
    ul.sidenav li a {
      float: left;
      padding: 15px;
    }
    
    div.content {margin-left: 0;}
  }

  @media screen and (max-width: 400px) {
    ul.sidenav li a {
      text-align: center;
      float: none;
    }
  }
</style>