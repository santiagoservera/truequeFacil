<template>
  <div class="home">
    <div class="container">
      <div class="row mx-0">
        <div class="col-lg-6">
          <div class="img-cont">
            <img alt="Vue logo" src="../assets/img/tuequeFacil.svg">
            <h2 class="text-center text-lg-start">Conecta con personas para poder hacer un trueque fácilmente!</h2>
          </div>
        </div>
        <div class="col-lg-6">
          <CardCom :btns="btnArray" class="mx-auto CardCom">
            <template #default>

              <form>
                <div class="mb-3 mt-2">
                  <input type="email" class="form-control" placeholder="Ingresa tu email">
                </div>
                <div class="mb-3 mt-2">
                  <input type="password" class="form-control" placeholder="Ingresa tu contraseña">
                </div>
              </form>

            </template>
            <template #footer>
              <hr/>
              <router-link class="btn btn-dark" to="/createAcount"><button  class="btn btn-dark">Registrate</button></router-link>
            </template>
          </CardCom>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CardCom from '@/components/CardCom.vue'

export default {
  name: 'HomeView',
  components: {
    CardCom
  },
  data() {
    return {
      btnArray:[
        {
        txt: 'Iniciar sesión',
        class: 'btn-success',
      },
      {
        txt: 'Olvidaste tu contrasena?',
        class: '',
      },
      

      ]
     
    }
  }
}
</script>

<style scoped>
h2{
  max-width: 470px;
  margin: auto;
  font-size: 1.8rem;
}
.home {
  margin: 4em auto;
  padding: 0 15px; /* Agregar un padding para dispositivos móviles */
}

.img-cont {
  display: flex;
  flex-direction: column;
}

img {
  max-width: 315px;
  margin: 1em auto 0 auto;
}

.CardCom {
  margin-top: 2.6em;
  max-width: 398px; /* Ancho máximo del componente CardCom */
}

.btn-dark{
  margin: auto;
  min-width: 195px;
}

@media (min-width: 992px) {
  img {
    margin: 0;
    margin-top: 5.6em;
  }
  h2 {
    margin: 0;
    margin-top: -0.8em;
    margin-left: 0.8em;
  }
  .CardCom{
    margin-top: 3rem;
  }
}
</style>
