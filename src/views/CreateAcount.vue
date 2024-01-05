<template>
    <div class="login">
        <div class="row mx-0">
            <div class="col-lg-6">
                <div class="img-cont">
                    <img alt="logo" src="../assets/img/tuequeFacil.svg" class="">
                    <h2 class="text-center text-lg-start">¡Crear una cuenta es facil y rapido!</h2>
                </div>
            </div>
            <div class="col-lg-6">
                <CardCom :btns="btnArray" class="mx-auto card-comp">
                    <template #default>
                        <form>
                            <div class="mb-3 mt-2">
                                <input class="form-control" type="text" placeholder="Ingrese su nombre"
                                    aria-label="default input example">
                            </div>
                            <div class="mb-3 mt-2">
                                <input class="form-control" type="text" placeholder="Ingrese su apellido"
                                    aria-label="default input example">
                            </div>
                            <div class="mb-3 mt-2">
                                <input class="form-control" type="text" placeholder="Localidad"
                                    aria-label="default input example">
                            </div>
                            <div class="mb-3 mt-2">
                                <input class="form-control" type="text" placeholder="Whatsapp"
                                    aria-label="default input example">
                            </div>
                            <div class="mb-3 mt-2">
                                <label for="formFileSm" class="form-label">Fecha de nacimiento</label>
                                <input class="form-control" type="date" placeholder="Whatsapp"
                                    aria-label="default input example">
                            </div>
                            <div class="mb-3 mt-2">
                                <label for="formFileSm" class="form-label">Foto de perfil</label>
                                <input class="form-control form-control-sm" id="formFileSm" type="file">
                            </div>
                            <div class="mb-3 mt-2">
                                <input type="password" class="form-control" placeholder="Ingresa su contraseña">
                            </div>
                            <div class="mb-3 mt-2">
                                <input type="password" class="form-control" placeholder="Repita su contraseña">
                            </div>
                        </form>
                    </template>
                    <template #footer>
                        <hr />
                        <router-link to="/login" class="btn btn-success"><button class="btn btn-success">Iniciar
                                sesion</button></router-link>
                    </template>

                </CardCom>

            </div>
        </div>
    </div>
</template>

<script>
import CardCom from "../components/CardCom.vue"
export default {
    components: {
        CardCom
    },
    data() {
        return {
            btnArray: [
                {
                    txt: "Registrarse",
                    class: 'btn-dark',
                },
                {
                    txt: "Ya posee cuenta? Inicie sesion",
                    class: '',
                }

            ],
        }
    },
}
</script>

<style scoped>
h2 {
    max-width: 470px;
    margin: auto;
    font-size: 1.8rem;
}

.login {
    max-width: 895px;
    margin: auto;
}

.img-cont {
    display: flex;
    flex-direction: column;
}

img {
    max-width: 315px;
    margin: 1em auto 0 auto;
}

.card-comp {
    max-width: 398px;
}

.btn-success {
    margin: auto;
    min-width: 195px;
}

@media (min-width: 992px) {
    .login {
        margin: 4em auto;
    }

    img {
        margin: 0;
        margin-top: 5.6em;
    }

    h2 {
        margin: 0;
        margin-top: -0.8em;
        margin-left: 0.8em;
    }

    
}</style>