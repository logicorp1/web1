<template>
  <div style="overflow-x: hidden">
    <br />
    <br />
    <div>
      <div style="position: relative">
        <div style="position: absolute; z-index: -1; object-fit:cover; width: 100%; height: 100%">
          <video autoplay loop muted playsinline class="video" poster="https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/plantilla1.jpg">
            <source src="https://ik.imagekit.io/qewkcqaku/tr:w-800/imagenes/proyect.mp4" type="video/mp4" />
          </video>
        </div>
        <div class="container" align="center">
          <br />
          <br class="d-none d-sm-none d-md-block" />
          <div class="row">
            <div class="col-12 col-sm-5 col-md-4 align-self-center">
              <h1 style="color: rgb(255, 102, 26)" align="left">
                Ingeniería de Proyectos Logísticos
              </h1>
              <p align="justify" style="color: white">
                es el conjunto de conocimientos, actitudes y herramientas de la
                gestión, que prestan apoyo al desarrollo más conveniente o más
                económico de la actividad empresarial, optimizando el resultado.
              </p>
            </div>
            <div class="col-0 col-sm-2 col-md-3"></div>
            <div align="justify" class="h-auto col-12 col-sm-5 col-md-5">
              <br class="d-block d-sm-none" />
              <div v-if="activador1">
                <div class="card2" color="transparent">
                  <div class="overlay"></div>
                  <NuxtLink
                    class="link"
                    to="#in1"
                    style="text-decoration: none; color: white"
                  >
                    <span style="white-space: normal">
                      <h4>1. Estudios preliminares de obra </h4>
                    </span>
                  </NuxtLink>
                </div>
                <div class="card2">
                  <div class="overlay"></div>
                  <NuxtLink
                    class="link"
                    to="#in2"
                    style="text-decoration: none; color: white"
                  >
                    <span style="white-space: normal">
                      <h4>2. Planos de Arquitectura</h4>
                    </span>
                  </NuxtLink>
                </div>
                <div class="card2">
                  <div class="overlay"></div>
                  <NuxtLink
                    class="link"
                    to="#in3"
                    style="text-decoration: none; color: white"
                  >
                    <span style="white-space: normal">
                      <h5>3. Planos de especialidades</h5>
                    </span>
                  </NuxtLink>
                </div>
                <div class="card2">
                  <div class="overlay"></div>
                  <NuxtLink
                    class="link"
                    to="#in7"
                    style="text-decoration: none; color: white"
                  >
                    <span style="white-space: normal">
                      <h5>4. Medición de Planitud de una Losa</h5>
                    </span>
                  </NuxtLink>
                </div>
                <div class="card2">
                  <div class="overlay"></div>
                  <NuxtLink
                    class="link"
                    to="#in4"
                    style="text-decoration: none; color: white"
                  >
                    <span style="white-space: normal">
                      <h5 align="justify">
                        5. Simuladores para Definir Sistemas de Almacenaje
                      </h5>
                    </span>
                  </NuxtLink>
                </div>
                <div class="card2">
                  <div class="overlay"></div>
                  <NuxtLink
                    class="link"
                    to="#in5"
                    style="text-decoration: none; color: white"
                  >
                    <span style="white-space: normal">
                      <h5>
                        6. Simuladores para Definir Equipos de Material Handling
                      </h5>
                    </span>
                  </NuxtLink>
                </div>
                <div class="card2">
                  <div class="overlay"></div>
                  <NuxtLink
                    class="link"
                    to="#in6"
                    style="text-decoration: none; color: white"
                  >
                    <span style="white-space: normal">
                      <h5>7. Simuladores para Picking</h5>
                    </span>
                  </NuxtLink>
                </div>
              </div>
              <div
                v-for="(card, index) in cards4"
                :key="index"
                v-if="!activador1"
              >
                <div
                  align="justify"
                  class="card2"
                  @click="showDialog(card)"
                  style="cursor: pointer"
                >
                  <div class="overlay"></div>
                  <span style="white-space: normal">
                    <h5 style="text-decoration: none; color: white">
                      {{ card.nom }}
                    </h5>
                  </span>
                </div>
              </div>
            </div>
          </div>
        </div>
        <br />
      </div>
      <!-- La cabecera con la info-->
      <div v-if="activador1">
        <div class="container">
          <br id="in1" />
          <br class="d-none d-sm-block" />

          <!--Estudio Mecanica de Suelos-->
          <br />
          <div v-scrolls>
              <div class="container">
                <div class="row card1">
                  <div align="center" class="align-self-center col-12 col-sm-6 order-2 order-sm-1">
                    <h1 align="center">Estudios preliminares de obra </h1>
                    <br />
                    <p
                      align="justify"
                      style="
                        padding-right: 3vh;
                        padding-left: 3vh;
                        font-size: 100%;
                      "
                    >
                      1. Estudio Mecanica de Suelos
                      <br />
                      <br />
                      2. Levantamiento Topografico
                      <br />
                      <br />
                      3. Levantamiento Arquitectonico
                      <br />
                      <br />
                      4. Sistema de Utilización en Media Tensión
                    </p>
                    <br />
                  </div>
                  <div
                    class="col-12 col-sm-6 order-1 order-sm-2"
                  >
                    <swiper :loop="true" style="max-height: 60vh; width:100%; color: black">
                      <swiper-slide v-for="card in cards" :key="card.src" class="d-flex align-items-center">
                        <img :src="card.src" class="d-flex align-items-center" style="width:100%; height: 100%; object-fit: contain" alt="..." />
                      </swiper-slide>
                      <div class="boton1">
                      <boton />
                    </div>
                    </swiper>
                  </div>
                </div>
              </div>
          </div>
          <br />
          <br id="in2" />
          <br class="d-none d-sm-block" />
          <br class="d-none d-sm-block" />
          <!--Planos de Arquitectura-->
          <br />
          <div v-scrolls>
            <div class="container">
              <div class="row card1">
                <div
                  class="col-12 col-sm-6"
                >
                  <swiper :loop="true" style="max-height: 60vh; color: black">
                    <swiper-slide v-for="card in cards1" :key="card.src" class="d-flex align-items-center">
                      <img :src="card.src" class="d-flex align-items-center" style="width:100%; height: 100%; object-fit: contain" alt="..." />
                    </swiper-slide>
                    <div class="boton1">
                    <boton />
                  </div>
                  </swiper>
                </div>
                <div align="center" class="align-self-center col-12 col-sm-6">
                  <h1 align="center">Planos de Arquitectura</h1>
                  <br />
                  <p
                    align="justify"
                    style="
                      padding-right: 3vh;
                      padding-left: 3vh;
                      font-size: 100%;
                    "
                  >
                    1. Desarrollo de AnteProyecto
                    <br />
                    <br />
                    2. Desarrollo de Proyecto
                    <br />
                    <br />
                    3. Modelado 3D.
                    <br />
                    <br />
                    4. Renderizado y Simulación 3D.
                  </p>
                  <br />
                </div>
              </div>
            </div>
          </div>
          <br class="d-none d-sm-block" />
          <br class="d-none d-sm-block" />
          <br id="in3" />
          <br />
          <!--Planos de Especialidades-->
          <div v-scrolls>
            <div class="container">
              <div class="row card1">
                <div
                  style="max-height: 50vh;"
                  class="col-12 col-sm-6 order-1 order-sm-2"
                >
                  <swiper :loop="true" style="height: 100%; color: black">
                    <swiper-slide v-for="card in cards5" :key="card" class="d-flex align-items-center">
                      <img :src="card" class="d-flex align-items-center" style="width:100%; height: 100%; object-fit: contain" alt="..." />
                    </swiper-slide>
                    <div class="boton1">
                    <boton />
                  </div>
                  </swiper>
                </div>
                <div align="center" class="align-self-center col-12 col-sm-6 order-2 order-sm-1">
                  <h1 align="center">Planos de especialidades</h1>
                  <br />
                  <p
                    align="justify"
                    style="
                      padding-right: 3vh;
                      padding-left: 3vh;
                      font-size: 100%;
                    "
                  >
                    1. Planos Estructurales
                    <br />
                    <br />
                    2. Planos Instalaciones Sanitarias
                    <br />
                    <br />
                    3. Planos Instalaciones Electricas
                    <br />
                    <br />
                    4. Planos de Data y Comunicaciones
                    <br />
                    <br />
                    5. Planos Mecánicos
                    <br />
                    <br />
                    6. Planos Sistema Contra Incendios
                  </p>
                  <br />
                </div>
              </div>
            </div>
          </div>
          <br class="d-none d-sm-block" />
          <br class="d-none d-sm-block" />
          <br id="in7" />
          <br />

          <!--Medición de Planitud de una Losa-->
          <br />
          <div>
            <div v-scrolls>
              <div class="card1">
              <div class="container">
                <div class="row">
                  <div
                    align="center"
                    class="col-12 align-self-center justify-center d-none d-sm-flex"
                  >
                    <h1 align="center">Medición de Planitud de una Losa</h1>
                    <br />
                  </div>
                  <div style="height: 350px; min-height: 287px" class="col-12">
                    <swiper :loop="true" style="height: 100%; color: black">
                    <swiper-slide v-for="card in cards2" :key="card.show" class="d-flex align-items-center">
                      <img :src="card.src" class="d-flex align-items-center" style="width:100%; height: 100%; object-fit: contain" alt="..." />
                    </swiper-slide>
                    <div class="boton1">
                    <boton />
                  </div>
                  </swiper>
                  </div>
                  <div
                    align="center"
                    class="col-12 align-self-center d-flex d-sm-none justify-center"
                  >
                    <h1 align="center">Medición de Planitud de una Losa</h1>
                    <br />
                  </div>
                </div>
              </div>
            </div>
            </div>
          </div>
          <br />
          <br id="in4" />
          <br />

          <!--Simuladores para Definir Sistemas de Almacenaje-->
          <div>
            <h1 align="center">
              Simuladores para Definir Sistemas de Almacenaje
            </h1>
            <br />
            <div class="row">
              <div
                class="col-12 col-md-6 col-sm-6"
                v-for="card in cards3"
                :key="card.id"
                align="center"
                v-scrolls
                style="padding-bottom: 25px"
              >
                <div
                  @click="showDialog(card)"
                  align="center"
                  style="width: 100%; cursor: pointer"
                  v-scrolls
                  class="card1"
                >
                  <div class="overlay"></div>
                  <img v-if="card.cover" :src="card.src" style="height: 300px; width: 100%; object-fit: cover; z-index: 999" />
                  <img v-if="!card.cover" style="height: 300px; width: 100%; object-fit: contain; z-index: 999" :src="card.src" />
                </div>
              </div>
            </div>
          </div>
          <br />
          <br />
          <div class="row">
            <!--Simuladores para Definir Equipos de Material Handling-->
            <div
              id="in5"
              class="col-12 col-md-6 col-sm-6"
              align="center"
              v-scrolls
            >
              <h1 align="center">
                Simuladores para Definir Material Handling
              </h1>
              <div
                @click="showDialog1()"
                elevation="21"
                align="center"
                style="width: 100%; cursor: pointer"
                v-scrolls
                class="card1"
              >
                <div class="overlay"></div>
                <img style="height: 300px; width: 100%; object-fit: contain; z-index: 999" :src="p6" :lazy-src="p6" />
              </div>
            </div>
            <!--Simuladores para Picking-->
            <div
              id="in6"
              align="center"
              v-scrolls
              class="col-12 col-md-6 col-sm-6"
            >
              <br />
              <h1>Simuladores para Picking</h1>
              <div
                @click="showDialog2()"
                align="center"
                v-scrolls
                class="card1"
                style="cursor: pointer; width: 100%"
              >
                <div class="overlay"></div>
                <img style="height: 300px; width: 100%; object-fit: contain; z-index: 999" :src="p7" />
              </div>
            </div>
          </div>
        </div>
        <br />
        <br />
      </div>
      <dibox v-show="show1" @close="hideDialog1()">
        <div outlined elevation="0">
          <div style="position: relative">
            <img style="width: 100%; height: 100%; object-fit: contain" :src="p6" :lazy-src="p6" />
            <div style="position: absolute; top: 0; right: 0">
              <button class="btn btn-danger" @click="hideDialog1()">
                <span class="mdi mdi-arrow-u-left-bottom" style="color: white"></span>
              </button>
            </div>
          </div>
        </div>
      </dibox>
      <dibox v-show="show2" @close="hideDialog2()">
        <div>
          <div style="position: relative">
            <img
              style="width: 100%; height: 100%; object-fit: contain"
              :src="p7"
            />
            <div style="position: absolute; top: 0; right: 0">
              <button class="btn btn-danger" @click="hideDialog2()">
                <span class="mdi mdi-arrow-u-left-bottom" style="color: white"></span>
              </button>
            </div>
          </div>
        </div>
      </dibox>
      <div v-for="(card, index) in cards4" :key="index" v-if="!activador1">
        <dibox v-show="card.show" @close="hideDialog(card)">
          <div class="row">
            <div class="col-0 col-md-1"></div>
            <div class="col-12 col-md-10" style="width: 90vw; height: 100%">
              <div
                class="alert alert-danger"
                role="alert"
                v-if="alert"
                transition="slide-y-transition"
              >
                Usuario o Contraseña Equivocado
              </div>
              <div class="d-flex justify-content-end">
                <button
                  type="button"
                  class="btn btn-danger"
                  @click="card.show = false"
                >
                  <span class="mdi mdi-arrow-u-left-bottom" style="color: white"></span>
                </button>
              </div>
              <div class="container">
                <div class="row" align="center">
                  <div align="center" class="register col-12">
                    <h2>Log in</h2>
                    <br />
                    <input
                      type="text"
                      placeholder="Username"
                      v-model="username"
                    />
                    <input
                      type="password"
                      placeholder="password"
                      v-model="password"
                    />
                    <button v-on:click="log2(card)">log in</button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </dibox>
      </div>
      <!--pie de pagina -->
    </div>
            <div v-for="card in cards3">
          <dibox v-show="card.show" @close="hideDialog(card)">
            <div style="position: relative">
                <img style="width: 100%; height: 100%; object-fit: contain" :src="card.src" />
                <div style="position: absolute; top: 0; right: 0">
                  <button
                    class="btn btn-danger"
                    @click="hideDialog(card)"
                  >
                    <span class="mdi mdi-arrow-u-left-bottom" style="color: white"></span>
                  </button>
                </div>
            </div>
          </dibox>
        </div>
    <pie />
  </div>
</template>

<script>
import { Navigation } from 'swiper';
import axios from "axios";
export default {
  name: "Ingenieria de proyectos logisticos",
  beforeMount() {
    this.activador = true;
    if (localStorage.getItem("token")) {
      this.activador1 = true;
    }
  },
  setup() {
    useHead({
      title: "Ingenieria de proyectos logisticos",
      meta: [
        {
          name: "robots",
          content: "index, follow",
        },
        {
          name: "description",
          content:
            "Somos un grupo de profesionales especializados en almacenes, contamos con más de 20 años",
        },
        {
          property: "site_name",
          content: "LogicorPeru",
        },
        {
          property: "og:title",
          content: "Ingenieria de proyectos logisticos",
        },
        {
          property: "og:description",
          content:
            "Somos un grupo de profesionales especializados en almacenes, contamos con más de 20 años",
        },
        {
          property: "og:image",
          content:
            "https://storage.icograms.com/templates/preview/warehouse-technology.png",
        },
        {
          property: "og:url",
          content: "/ingenieria",
        },
        {
          name: "twitter:card",
          content: "summary_large_image",
        },
        {
          name: "twitter:tittle",
          content: "Ingenieria de proyectos logisticos",
        },
        {
          name: "twitter:description",
          content:
            "Somos un grupo de profesionales especializados en almacenes, contamos con más de 20 años",
        },
        {
          name: "twitter:image",
          content:
            "https://storage.icograms.com/templates/preview/warehouse-technology.png",
        },
      ],
    });
    return {
        modules: [Navigation],
      };
  },
  unmounted() {
    document.body.style.position = "static";
    document.body.style.top = "";
    document.body.style.width = "";
    document.body.style.overflowY = "";
    window.scrollTo({top: this.scrollPosition, behavior: "instant"});
  },
  data() {
    return {
      scrollPosition: 0,
      show1: false,
      show2: false,
      activador1: false,
      activador: false,
      state: false,
      alert: false,
      p1: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/ingenieria1.png",
      p2: "https://ik.imagekit.io/qewkcqaku/tr:w-800/imagenes/Multimedia3.mp4",
      p3: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/ingenieria2.png",
      p4: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/ingenieria3.png",
      p5: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto52.jpg",
      p6: "https://ik.imagekit.io/qewkcqaku/tr:w-800/imagenes/proyecto60.jpg",
      p7: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto61.jpg",
      p8: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto54.jpg",
      username: "",
      password: "",
      slides: ["First", "Second", "Third", "Fourth", "Fifth"],
      cards: [
        { id: 1, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto48.jpg", cover: true },
        { id: 2, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto49.jpg", cover: true },
        { id: 3, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto50.jpg", cover: true },
        { id: 4, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto51.jpg", cover: false },
      ],
      cards1: [
        { id: 1, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto53.jpg", cover: false },
        { id: 2, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto54.jpg", cover: false },
        { id: 3, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto55.jpg", cover: false },
        { id: 4, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto56.jpg", cover: false },
      ],
      cards2: [
        { id: 1, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/losa1.png", cover: true },
        { id: 2, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/losa2.png", cover: true },
        { id: 3, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/supervision3.jpg", cover: false },
        { id: 4, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/supervision4.jpg", cover: false },
        { id: 5, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/supervision5.jpg", cover: false },
        { id: 6, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/supervision6.jpg", cover: false },
        { id: 7, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto57.jpg", cover: false },
      ],
      cards3: [
        { id: 1, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-800/imagenes/proyecto58.jpg", cover: false },
        { id: 2, show: false, src: "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/proyecto59.jpg", cover: false },
      ],
      cards4: [
        { nom: "1. Estudios preliminares de obra", tit: "#in1", show: false },
        { nom: "2. Planos de Arquitectura", tit: "#in2", show: false },
        { nom: "3. Planos de especialidades", tit: "#in3", show: false },
        {
          nom: "4. Medición de Planitud de una Losa",
          tit: "#in7",
          show: false,
        },
        {
          nom: "5. Simuladores para Definir Sistemas de Almacenaje",
          tit: "#in4",
          show: false,
        },
        {
          nom: "6. Simuladores para Definir Equipos de Material Handling",
          tit: "#in5",
          show: false,
        },
        { nom: "7. Simuladores para Picking", tit: "#in6", show: false },
      ],
      cards5: ["https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/planos.png", "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/planos1.png", "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/planos2.png", "https://ik.imagekit.io/qewkcqaku/tr:w-700/imagenes/planos3.png"],
    };
  },
  methods: {
    async log2(card) {
      const element = document.getElementById(card.tit);
      let result = await axios
        .post("https://python1-0y99.onrender.com/login", {
          username: this.username,
          password: this.password,
        })
        .catch((error) => {
          console.log(error);
          this.alert = true;
          setTimeout(() => {
            this.alert = false;
          }, 5000);
          this.username = "";
          this.password = "";
        });
      if (result.data.success == true) {
        card.show = false;
        document.body.style.position = "static";
        document.body.style.top = "";
        document.body.style.width = "";
        document.body.style.overflowY = "";
        window.scrollTo(0, this.scrollPosition);
        this.username = "";
        this.password = "";
        this.state = true;
        this.activador1 = true;
        this.$bus.$emit("activador", this.state);
        localStorage.setItem("token", true);
        card.show = false;
        return navigateTo(card.tit);
      }
    },
    showDialog(card) {
      this.scrollPosition = window.pageYOffset;
      card.show = true;
      document.body.style.position = "fixed";
      document.body.style.top = `-${this.scrollPosition}px`;
      document.body.style.width = "100%";
      document.body.style.overflowY = "scroll";
    },
    showDialog1() {
      this.scrollPosition = window.pageYOffset;
      this.show1 = true;
      document.body.style.position = "fixed";
      document.body.style.top = `-${this.scrollPosition}px`;
      document.body.style.width = "100%";
      document.body.style.overflowY = "scroll";
    },
    showDialog2() {
      this.scrollPosition = window.pageYOffset;
      this.show2 = true;
      document.body.style.position = "fixed";
      document.body.style.top = `-${this.scrollPosition}px`;
      document.body.style.width = "100%";
      document.body.style.overflowY = "scroll";
    },
    hideDialog(card) {
      card.show = false;
      document.body.style.position = "static";
      document.body.style.top = "";
      document.body.style.width = "";
      document.body.style.overflowY = "";
      window.scrollTo({top: this.scrollPosition, behavior: "instant"});
    },
    hideDialog1() {
      this.show1 = false;
      document.body.style.position = "static";
      document.body.style.top = "";
      document.body.style.width = "";
      document.body.style.overflowY = "";
      window.scrollTo({top: this.scrollPosition, behavior: "instant"});
    },
    hideDialog2() {
      this.show2 = false;
      document.body.style.position = "static";
      document.body.style.top = "";
      document.body.style.width = "";
      document.body.style.overflowY = "";
      window.scrollTo({top: this.scrollPosition, behavior: "instant"});
    },
  },
};
</script>

<style scoped>
  .boton1 {
    transition: opacity 0.3s ease-in-out;
    opacity: 0;
    position: absolute; 
    top: 30px; 
    width: 100%; 
    height: 100%
  }
  .swiper:hover .boton1 {
  opacity: 1
}
.card1 {
  background-color: #fff;
  border-radius: 4px;
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  overflow: hidden;
  position: relative;
}
.card2 {
  background-color: transparent;
  border-radius: 4px;
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  overflow: hidden;
  z-index: 2;
  position: relative;
}
.card2:hover .overlay {
  opacity: 1;
  z-index: -1;
  background-color: rgba(129, 129, 129, 0.171);
}
.card1:hover .overlay {
  opacity: 1;
  z-index: -1;
  background-color: rgba(129, 129, 129, 0.171);
}
.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
}
.video {
  filter: brightness(45%);
  height: 100%;
  width: 100%;
  object-fit: cover;
  display: block;
}

.before-enter {
  opacity: 0;
  transform: translateX(100px);
  transition: all 1s ease-out;
}
.enter {
  opacity: 1;
  transform: translateX(0px);
}
.register input {
  width: 100%;
  height: 40px;
  display: block;
  margin-bottom: 30px;
  padding-left: 20px;
  border: 1px solid #535353;
  border-radius: 5px;
}
.register button {
  width: 100%;
  height: 40px;
  display: block;
  margin-bottom: 30px;
  background-color: #000000;
  color: #fff;
  border: none;
  border-radius: 5px;
}
.register h2 {
  font-size: 32px;
  font-weight: 300;
  text-transform: uppercase;
}
</style>
