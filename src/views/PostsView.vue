<template>
  <div class="posts container">
    <div class="row mb-3">
      <img src="../assets/img/tuequeFacil.svg" alt="truequeFacil" class="logo">
      <!-- Campo de búsqueda -->
      <div class="col-lg-6 d-flex align-items-center justify-content-center">
        <div class="input-group">
          <input type="text" class="form-control" placeholder="Buscar..." v-model="searchQuery"
            @keyup.enter="performSearch">
          <button class="btn btn-success" type="button" @click="performSearch">Buscar</button>
        </div>
      </div>
     
      
    </div>

    <!-- Aquí se mantienen tus tarjetas de posts -->
    <div class="row ">
      
        <CardCom 
     title="Casa moderna"
     class="mt-2 mx-auto single-post col-lg-4 col-md-6"
     picture="https://images.pexels.com/photos/19541342/pexels-photo-19541342/free-photo-of-casas-casa-ventanas-ventana.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
     parrafo="permuto por terreno"
     :header ="{name: 'Sebastian Maikol', picture: 'https://randomuser.me/api/portraits/men/71.jpg'}"
     :likes="true"
     />
     
  
      <CardCom 
     title="Moto Personalizada"
     class="mt-2 mx-auto single-post col-lg-4 col-md-6"
     picture="https://images.pexels.com/photos/1715193/pexels-photo-1715193.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
     parrafo="permuto por auto"
     :header ="{name: 'Ricardo Sanchez', picture:'https://randomuser.me/api/portraits/men/81.jpg'}"
     :likes="true"
     />
     
      <CardCom 
     class="mt-2 mx-auto single-post col-lg-4 col-md-6"
     title="Bicicleta antigua"
     picture="https://images.pexels.com/photos/1431117/pexels-photo-1431117.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
     parrafo="Celular con wtsp"
     :header ="{name: 'Eliana Palacios', picture:'https://randomuser.me/api/portraits/women/90.jpg'}"
     :likes="true"
     />
   
     
      <CardCom 
     title="Moto Personalizada"
     class="mt-2 mx-auto single-post col-lg-4 col-md-6"
     picture="https://images.pexels.com/photos/1715193/pexels-photo-1715193.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
     parrafo="permuto por auto"
     :header ="{name: 'Ricardo Sanchez', picture:'https://randomuser.me/api/portraits/men/81.jpg'}"
     :likes="true"
     />
     
     
      <CardCom 
      title="Moto Personalizada"
      class="mt-2 mx-auto single-post col-lg-4 col-md-6 "
      picture="https://images.pexels.com/photos/1715193/pexels-photo-1715193.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
      parrafo="permuto por auto"
      :header ="{name: 'Ricardo Sanchez', picture:'https://randomuser.me/api/portraits/men/81.jpg'}"
      :likes="true"
      />
     
    

      <CardCom 
     title="Moto Personalizada"
     class="mt-2 mx-auto single-post col-lg-4 col-md-6"
     picture="https://images.pexels.com/photos/1715193/pexels-photo-1715193.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
     parrafo="permuto por auto"
     :header ="{name: 'Ricardo Sanchez', picture:'https://randomuser.me/api/portraits/men/81.jpg'}"
     :likes="true"
     />

    
     
    </div>
  </div>
</template>

<script>
import CardCom from "../components/CardCom.vue";
export default {
  components: {
    CardCom // Asegúrate de registrar el componente en la sección 'components'
  },
  name: 'PostsView',
  
}
</script>

<style scoped>
/* Estilos existentes */



.logo {
  max-width: 180px;
  padding: 0.2rem;
}

.single-post {
  max-width: 550px;
  height: 100%;
  overflow: hidden;
}

.single-post img {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Ajusta la imagen dentro del tamaño definido */
}
@media screen and (max-width: 768px) {
  .single-post {
    max-width: 100%; /* Ajustar ancho al 100% para dispositivos móviles */
    margin-bottom: 20px; /* Espaciado entre tarjetas */
  }
}





/* Estilos para las tarjetas */
.custom-link .single-post {
  /* Ajusta el tamaño de las tarjetas */
  max-width: 100%;
  height: 500px; /* Modifica la altura según sea necesario */
  overflow: hidden;
  margin-bottom: 20px; /* Espaciado entre tarjetas */
}

</style>
