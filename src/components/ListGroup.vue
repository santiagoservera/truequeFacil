<template>
    <ul class="list-group">
      <li class="list-group-item text-muted">A 4 personas les gusta esto</li>
      <li class="list-group-item">
        <div class="d-flex justify-content-between">
          <button class="btn btn-success small-btn">
            <span class="material-icons-round">thumb_up</span>Me gusta
          </button>
          <button class="btn btn-primary small-btn">
            <span class="material-icons-round">question_answer</span>Comentar
          </button>
          <router-link to="/detail">
            <button class="btn btn-dark small-btn">
              <span class="material-icons-round">read_more</span>Ver más
            </button>
          </router-link>
        </div>
      </li>
    </ul>
  </template>
  
  <script>
  export default {
  
  }
  </script>
  
  <style scoped>
  .small-btn {
    font-size: 12px; /* Ajusta el tamaño de fuente según lo necesites */
    padding: 5px 10px; /* Ajusta el relleno (padding) según lo necesites */
  }
  </style>
  