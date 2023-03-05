<template>
  <router-view/>
</template>



<style lang="scss">
* { 
    text-decoration: none;
    margin: 0;
    padding: 0;
    list-style: none;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

._anim-items {
  transform: translate(-100px, 50px);
  opacity: 0;
  transition: 0.8s ease 0s;
}
._activeScroll {
  transform: translate(0, 0);
  opacity: 1;
}
nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
