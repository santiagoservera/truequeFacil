<template>
    <footer class="mt-5">
      <ul class="list-group list-group-flush list-group-horizontal text-center mb-0">
        <li class="list-group-item">
          <router-link class="router-link" to="/">Publicaciones</router-link>
        </li>
        <li class="list-group-item">
          <router-link class="router-link" to="/about">Acerca de nosotros</router-link>
        </li>
        <li class="list-group-item">
          <router-link class="router-link" to="/home">Inicia sesión</router-link>
        </li>
      </ul>
      <div class="text-center" id="copyright">TruequeFacil &#169; 2024</div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'FooterCom',
  }
  </script>
  
  <style scoped>
  footer {
    width: 100%;
    position: relative; /* Cambio la posición a relativa */
  }
  
  .text-center {
    margin-top: 1em; /* Aumento el espacio superior */
    margin-bottom: 0.5em;
  }
  
  .list-group {
    justify-content: center;
  }
  
  .list-group-item {
    border: none;
  }
  
  .router-link {
    text-decoration: none;
  }
  
  /* Nuevos estilos para el copyright */
  #copyright {
    position: relative;
    bottom: 5px; /* Ajusto la distancia desde abajo */
    left: 50%; /* Centro horizontalmente */
    transform: translateX(-50%); /* Centro horizontalmente */
    font-size: 12px; /* Tamaño de fuente más pequeño */
    color: #888; /* Color del texto más claro */
  }
  </style>
  