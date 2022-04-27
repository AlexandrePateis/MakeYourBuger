<template>
  <div id="nav">
    <router-link to="/" id="logo_url">
      <img :src="logo" id="logo" :alt="alt" />
      <p class="title">MakeYouBurger</p>
    </router-link>
    <div class="menus">
      <router-link to="/">Home</router-link>
      <router-link to="/pedidos">Pedidos</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  props: ["logo", "alt"],
};
</script>

<style scoped>
#nav {
  background-color: rgb(0, 0, 0);
  border-bottom: 4px solid rgb(0, 0, 0);
  padding: 15px 50px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#nav a {
  text-decoration: none;
  color: white;
  margin: 15px;
  transition: linear 0.3s;
}
#nav a:hover{
  color: yellow;
}
#logo_url{
  display: flex;
  align-items: center;
  justify-content: center;
}
.title{
  cursor:pointer;
  padding: 0;
  margin-left: 1em;
  font-size: 2em;
}
.menus{
  font-size: 1.5em;
}
</style>
