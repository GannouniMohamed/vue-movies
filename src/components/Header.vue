<template>
  <header>
    <ul class="sidenav">
      <li v-for="linkItem in navListLinks" :key="linkItem.text">
        <a
          v-bind:class="{ active: activeTab === linkItem.text  }"
          :href="linkItem.href"
          v-on:click="setActiveTab(linkItem.text)"
          >
          <font-awesome-icon v-bind:icon="linkItem.icon" /> {{linkItem.text}}
        </a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      activeTab: 'HOME',
      navListLinks: [
        { isActive: false, href: '/home', icon: 'home', text: 'HOME' },
        { isActive: false, href: '/movies', icon: 'film', text: 'MOVIES' },
        { isActive: false, href: '/series', icon: 'tv', text: 'SERIES' },
      ],
    };
  },
  methods: {
    setActiveTab(tab) {
      this.activeTab = tab;
    },
  },
};
</script>

<style scoped>
header {
  margin: 0;
  height: 56px;
  padding: 0 16px 0 24px;
  color: #ffffff;
  background-color: #ffffff;
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;
  width: 100%;
  top: 0px;
  -webkit-box-shadow: 2px 1px 19px 0px rgba(0,0,0,0.75);
  -moz-box-shadow: 2px 1px 19px 0px rgba(0,0,0,0.75);
  box-shadow: 2px 1px 19px 0px rgba(0,0,0,0.75);
  z-index: 999999;
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
    color: #897f76;
    padding: 8px 16px;
    text-decoration: none;
  }
  
  ul.sidenav li a.active {
    color: #FF7E00 !important;
    border-color: #FF7E00;
    border-bottom: 3px solid #FF7E00;
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