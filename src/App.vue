<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header id="cabecalho">
    <button class="item" id="btn_opt"><img id="icon_menu" src="https://cdn-icons-png.flaticon.com/512/1243/1243926.png?w=740&t=st=1673358784~exp=1673359384~hmac=fda79b37e4d733221221de79d9f947768508a5e6cebfa6353ac6bf8e6cb4216f"></button>

    <nav class="item" id="barra_nav">
      <RouterLink to="/">Inicio</RouterLink>
      <RouterLink to="/about">Info</RouterLink>
    </nav>

    <div id="foto_corsol"><img  id="logo_corsol" src="https://corsolar.com.br/wp-content/uploads/2022/03/corsolar-logo.png"></div>

    <div id="last-line"></div>
  </header>


  <RouterView />
</template>

<style scoped>
nav a.router-link-exact-active {
  color: var(--color-text);
}
nav a.router-link-exact-active:hover {
  background-color: transparent;
}
nav a {

  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}
nav a:first-of-type {
  border: 0;
}
</style>
