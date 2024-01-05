<template>
    <div class="row container-post">
      <div class="col-lg-6">
        <CardCom
          title="Casa moderna"
          class="mt-2 mx-auto col card-body full-image "
          picture="https://images.pexels.com/photos/19541342/pexels-photo-19541342/free-photo-of-casas-casa-ventanas-ventana.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
          parrafo="permuto por terreno medianamente grande."
          :header="{ name: 'Sebastian Maikol', picture: 'https://randomuser.me/api/portraits/men/71.jpg' }"
          :detailView="true"
        />
      </div>
  
      <div class="col-lg-6">
        <div class="card mt-4">
          <div class="card-header">
            <h5>Datos del contacto</h5>
          </div>
          <div class="card-body">
            <p><strong>Nombre:</strong> Sebastian Maikol</p>
            <p><strong>Email:</strong> example@example.com</p>
            <p><strong>Teléfono:</strong> +123456789</p>
            <p><strong>Dirección:</strong> Rivadavia 1923 (S)</p>
            <iframe
                                src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d13602.424021002293!2d-68.51796891188309!3d-31.53497950125574!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e0!3m2!1ses!2sar!4v1704482031577!5m2!1ses!2sar"
                                class="w-100" height="250" loading="lazy"></iframe>
            <!-- Agrega más detalles del contacto según sea necesario -->
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import CardCom from "../components/CardCom.vue";
  export default {
    components: {
      CardCom // Asegúrate de registrar el componente en la sección 'components'
    },
    name: 'DetailView'
  }
  </script>
  
  <style scoped>
  .container-post {
    padding: 20px;
  }
  
  @media screen and (max-width: 768px) {
    .single-post {
      margin-bottom: 20px;
    }
  
    .mt-4 {
      margin-top: 1rem;
    }
  }
  
  .card-img-top {
    width: 100%;
    height: auto;
    object-fit: contain;
    max-height: 500px; /* Ajusta la altura máxima según tus necesidades */
  }
  
  /* Estilos para la tarjeta de contacto */
  .card {
    border: none;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1), 0 8px 16px rgba(0, 0, 0, 0.1);
  }
  
  .card-header {
    background-color: transparent;
    padding: 10px 20px;
    border-bottom: none;
  }
  
  .card-header h5 {
    font-size: 1.25rem;
    margin-bottom: 0;
  }
  
  .card-body {
    padding: 20px;
  }
  
  .card-body p {
    margin-bottom: 10px;
    font-size: 1rem;
  }

 
  

  .container-post {
    padding: 20px;
  }
  </style>
  