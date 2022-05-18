<template>
  <div>
    <p class="logo">4PRINT</p>
  </div>
  <div id="nav">
    <router-link to="/" class="router">INÍCIO</router-link>
    <router-link to="/sobre" class="router">SOBRE</router-link>
    <router-link to="/contato" class="router">CONTATO</router-link>
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>

<style lang="scss">
#app {
  font-family: 'Montserrat', sans-serif;
}

.logo {
  display: flex;
  color: white;
  width: 100px;
  position: relative;
  z-index: 1;
  padding: 16px 0;
  margin-left: 15%;
  font-size: 20px;
}

.router {
  margin-right: 20px;
}

#nav {
  padding: 16px 0;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  background-color: rgb(30, 30, 30);
  color: white;
  text-align: center;

  a {
    color: white;
    text-decoration: none;
    transition: color .15s;
    font-size: .77em;

    &.router-link-exact-active {
      color: #007bff;
    }
  }
  a:hover{
    color: #1988ff;
  }
}
</style>
