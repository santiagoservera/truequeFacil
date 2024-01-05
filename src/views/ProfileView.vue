<template>
    <div class="container py-5 h-100">
        <div class="row d-flex justify-content-center align-items-center h-100">
            <div class="col-md-12 col-xl-4">
                <div class="card" style="border-radius: 15px;">
                    <div class="card-body text-center">
                        <div class="mt-3 mb-4">
                            <img src="https://randomuser.me/api/portraits/men/81.jpg" class="rounded-circle img-fluid"
                                style="width: 100px;" />
                        </div>
                        <h4 class="mb-2">Sebastian Maikol</h4>
                        <p class="text-muted mb-4">"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                            eiusmod tempor incididunt ut labore et dolore magna aliqua.
                            Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
                            commodo consequat."</p>
                        <div class="mb-4 pb-2">
                            <button type="button" class="btn btn-outline-success btn-floating border-0">
                                <img src="../assets/img/facebook.svg" alt="Facebook" class="img-fluid">
                            </button>
                            <button type="button" class="btn btn-outline-success btn-floating border-0">
                                <img src="../assets/img/twitter.svg" alt="Twitter" class="img-fluid">
                            </button>
                            <button type="button" class="btn btn-outline-success btn-floating border-0">
                                <img src="../assets/img/instagram.svg" alt="Instagram" class="img-fluid">
                            </button>
                        </div>
                        <div class="row">
                            <div class="col-md-4 col-sm-12 mb-4">
                                <div class="progress blue">
                                    <span class="progress-left">
                                        <span class="progress-bar"></span>
                                    </span>
                                    <span class="progress-right">
                                        <span class="progress-bar"></span>
                                    </span>
                                    <div class="progress-value">90%</div>
                                </div>
                                <div class="text-center">
                                    <p>Seguridad</p>
                                </div>
                            </div>

                            <div class="col-md-4 col-sm-12 mb-4">
                                <div class="progress blue">
                                    <span class="progress-left">
                                        <span class="progress-bar"></span>
                                    </span>
                                    <span class="progress-right">
                                        <span class="progress-bar"></span>
                                    </span>
                                    <div class="progress-value">90%</div>
                                </div>
                                <div class="text-center">
                                    <p>Confianza</p>
                                </div>
                            </div>
                            <div class="col-md-4 col-sm-12 mb-4">
                                <div class="progress blue">
                                    <span class="progress-left">
                                        <span class="progress-bar"></span>
                                    </span>
                                    <span class="progress-right">
                                        <span class="progress-bar"></span>
                                    </span>
                                    <div class="progress-value">50%</div>
                                </div>
                                <div class="text-center">
                                    <p>Amabilidad</p>
                                </div>
                            </div>
                        </div>
                        <div class="d-flex justify-content-between text-center mt-5 mb-2">
                            <div>
                                <p class="mb-2 h5">8471</p>
                                <p class="text-muted mb-0">Seguidores</p>
                            </div>
                            <div class="px-3">
                                <p class="mb-2 h5">8512</p>
                                <p class="text-muted mb-0">Seguidos</p>
                            </div>
                            <div>
                                <p class="mb-2 h5">51</p>
                                <p class="text-muted mb-0">Post</p>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "ProfileView",
}
</script>

<style scoped>
.progress {
    width: 100px;
    height: 100px;
    line-height: 100px;
    background: none;
    margin: 0 auto;
    box-shadow: none;
    position: relative;
}

.progress:after {
    content: "";
    width: 100%;
    height: 100%;
    border-radius: 50%;
    border: 12px solid #fff;
    position: absolute;
    top: 0;
    left: 0;
}

.progress>span {
    width: 50%;
    height: 100%;
    overflow: hidden;
    position: absolute;
    top: 0;
    z-index: 1;
}

.progress .progress-left {
    left: 0;
}

.progress .progress-bar {
    width: 100%;
    height: 100%;
    background: none;
    border-width: 6px;
    border-style: solid;
    position: absolute;
    top: 0;
}

.progress .progress-left .progress-bar {
    left: 100%;
    border-top-right-radius: 80px;
    border-bottom-right-radius: 80px;
    border-left: 0;
    -webkit-transform-origin: center left;
    transform-origin: center left;
}

.progress .progress-right {
    right: 0;
}

.progress .progress-right .progress-bar {
    left: -100%;
    border-top-left-radius: 80px;
    border-bottom-left-radius: 80px;
    border-right: 0;
    -webkit-transform-origin: center right;
    transform-origin: center right;
    animation: loading-1 1.8s linear forwards;
}

.progress .progress-value {
    width: 90%;
    height: 100%;
    border-radius: 50%;
    background: #ffffff;
    font-size: 24px;
    color: #000000;
    line-height: 135px;
    text-align: center;
    position: absolute;
    top: -20%;
    left: 5%;
}

.progress.blue .progress-bar {
    border-color: #65A386;
}

.progress.blue .progress-left .progress-bar {
    animation: loading-2 1.5s linear forwards 1.8s;
}






@keyframes loading-1 {
    0% {
        -webkit-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    100% {
        -webkit-transform: rotate(180deg);
        transform: rotate(180deg);
    }
}

@keyframes loading-2 {
    0% {
        -webkit-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    100% {
        -webkit-transform: rotate(144deg);
        transform: rotate(144deg);
    }
}

@keyframes loading-3 {
    0% {
        -webkit-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    100% {
        -webkit-transform: rotate(90deg);
        transform: rotate(90deg);
    }
}

@keyframes loading-4 {
    0% {
        -webkit-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    100% {
        -webkit-transform: rotate(36deg);
        transform: rotate(36deg);
    }
}

@keyframes loading-5 {
    0% {
        -webkit-transform: rotate(0deg);
        transform: rotate(0deg);
    }

    100% {
        -webkit-transform: rotate(126deg);
        transform: rotate(126deg);
    }
}
</style>