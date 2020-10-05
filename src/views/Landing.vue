<template>
  <div class="relative">
    <nav
      id="nav"
      class="absolute w-full z-40 pt-12 px-4 md:pt-4 md:px-8 lg:pt-16 lg-px-12 rounded-b-large"
      v-bind:class="{ 'bg-white': Menu == false }"
    >
      <div class="druk-bold text-3xl float-left lg:mt-1">Foodies</div>
      <div class="block float-right lg:hidden">
        <button
          id="nav-toggle"
          v-on:click="Menu = false"
          v-if="Menu == true"
          class="flex float left items-center px-3 "
        >
          <img
            src="@/assets/landing/menu.svg"
            class="float-right w-auto pt-1"
          />
        </button>
        <button
          id="nav-toggle"
          v-on:click="Menu = true"
          v-if="Menu == false"
          class="flex float left items-center px-3 "
        >
          <img
            src="@/assets/landing/close.svg"
            class="float-right w-auto pt-1"
          />
        </button>
      </div>
      <div
        class="w-full flex-grow pt-6 lg:pt-0"
        v-bind:class="{ hidden: Menu }"
        id="nav-content"
      >
        <ul class="lg:flex justify-end flex-1 items-center">
          <li class="mr-3">
            <a class="inline-block "></a>
          </li>
          <li class="mr-3">
            <a class="inline-block syne text-2xl pt-12 px-4" href="#"
              >Acerca de</a
            >
          </li>
          <li class="mr-3">
            <a class="inline-block text-2xl syne pt-12 px-4" href="#"
              >Restaurantes</a
            >
          </li>
          <li class="mr-3">
            <a class="inline-block syne text-2xl pt-12 pb-12 px-4" href="#"
              >Contáctanos</a
            >
          </li>
        </ul>
      </div>
      <div class="mt-4 lg:ml-24 float-left invisible lg:visible">
        <div class="syne text-xl mx-6 float-left invisible lg:visible">
          Acerca de
        </div>
        <div class="syne text-xl mx-6 float-left invisible lg:visible">
          Restaurantes
        </div>
        <div class="syne text-xl mx-6 float-left invisible lg:visible">
          Menú
        </div>
        <div class="syne text-xl mx-6 float-left invisible lg:visible">
          Contáctanos
        </div>
      </div>
    </nav>
    <div id="background" class="absolute top-0 z-0 w-full">
      <img
        src="@/assets/landing/vector.svg"
        class="float-right w-full pl-1 md:w-7/12 lg:w-6.5/12"
      />
    </div>
    <div id="content" class="relative z-10 w-full h-full pt-24 lg:pt-40">
      <!-- <div class="bg-black mx-auto h-screen w-1 z-10"></div> -->
      <div id="section-1" class="pl-8 pr-2 ">
        <div
          class="container w-full md:w-1/2 md:float-right"
          data-aos="zoom-in"
        >
          <img src="@/assets/landing/burger.svg" class="md:w-10/12" />
        </div>
        <div class="container pt-10 w-full md:w-1/2">
          <div class="relative">
            <div
              class="relative z-10 leading-9 lg:leading-none druk-bold text-3.5xl md:text-4.5xl md:w-11/12 lg:text-6.5xl lg:w-10/12"
            >
              Un nuevo sabor esta en la ciudad
            </div>
            <img
              src="@/assets/landing/bg_text.svg"
              class="absolute bottom-0 left-0 z-0 w-auto md:w-10/12 "
            />
          </div>
          <div class="open-gray mt-8 mr-12 md:mr-20 lg:text-lg">
            Estamos a punto de descubrir un mundo lleno de sabores y de
            emociones inigualables.
          </div>
          <div class="syne mt-8 text-2xl">
            <p class="block float-left">Encuentranos</p>
            <img
              src="@/assets/landing/arrow.svg"
              class="float-left ml-4 mt-2 "
            />
          </div>
        </div>
      </div>
      <div id="section-2" class="mt-24 md:mt-48 md:pb-24 lg:mt-64 lg:pt-24 overflow-hidden lg:grid-cols-2">
        <div class="relative lg:w-6/12 lg:float-left">
          <img src="@/assets/landing/people.svg" class="max-w-none lg:max-w-full" />
          <div
            class="absolute bottom-0 right-0 druk-bold text-white mr-2 md:mr-12 ml-4 md:ml-32 mb-8 text-right leading-9 text-4.5xl md:text-4.5xl"
          >
            <p class="inline md:block">La comida es</p>
            <p class="inline text-yellow">nuestro arte</p>
          </div>
        </div>
        <div class="relative lg:w-6/12 lg:float-left">
          <div class="relative pl-8 pr-2 z-10 pt-20">
            <div class="syne mt-16 text-2xl">
              ¿Quién es Foodies?
            </div>
            <div class="open-gray mt-6">
              Elit irure ad nulla id elit laborum nostrud mollit irure. Velit
              reprehenderit sunt nulla enim aliquip duis tempor est culpa fugiat
              consequat culpa consectetur Lorem. Reprehenderit dolore culpa
              irure eiusmod minim occaecat et id minim ullamco.
            </div>
            <div
              class="relative z-10 syne mt-8 text-2xl md:text-xl "
            >
              <p class="float-left mr-4">Contáctanos</p>
              <img
                src="@/assets/landing/arrow.svg"
                class="float-left mt-2 md:mt-1"
              />
            </div>
          </div>
          <div class="absolute ribon invisible md:visible z-0">
            <img src="@/assets/landing/ribon.svg" class="" />
          </div>
        </div>
      </div>
      <div id="section-3" class="mt-10 grid grid-cols-1 md:grid-cols-2">
        <div id="directions" class="lg:col-span-1">
          <div
            class="leading-9 druk-bold text-3.5xl pl-8 pr-16 pb-8 md:text-4.5xl"
          >
            Estamos para ti
          </div>
          <div class="grid grid-cols-2">
            <div
              class="grid grid-cols-4 bg-black text-white h-12 content-center"
              v-on:click="selected=true"
            >
              <img
                src="@/assets/landing/burger-ico.svg"
                class="mt-1 mr-1 md:w-6 justify-self-end"
              />
              <p class="col-span-3 syne md:text-2xl">Para llevar</p>
            </div>
            <div
              class="grid grid-cols-4 text-black h-12 content-center border border-gray-500"
              v-on:click="selected=false"
            >
              <img
                src="@/assets/landing/delivery.svg"
                class=" mt-1 mr-1 md:w-10 justify-self-end"
              />
              <p class="col-span-3 syne md:text-2xl">Domicilio</p>
            </div>
            <div
              class="grid grid-cols-7 col-span-2 h-12 content-center border border-gray-500"
            >
              <img
                src="@/assets/landing/search.svg"
                class=" mt-2 mr-1 justify-self-end"
              />
              <input
                type="search"
                class="input p-3 col-span-6 h-full"
                placeholder="Buscar nombre o dirección"
              />
            </div>
          </div>
          <div class="mt-2 px-4" v-if="selected">
            <div
              class="directions rounded border border-black hover:border-transparent hover:bg-yellow-200 pl-3 pt-4 mb-3"
              v-for="delivery in delivery" v-bind:key="delivery"
            >
              <p class="syne text-lg mb-1">{{delivery.name}}</p>
              <p class="open text-sm">Abierto de {{delivery.opening_time}} - {{delivery.closing_time}}</p>
              <p class="open text-sm">
                {{delivery.address}}
              </p>
            </div>
          </div>
          <div class="mt-2 px-4" v-if="selected==false">
            <div
              class="directions rounded border border-black hover:border-transparent hover:bg-yellow-200 pl-3 pt-4 mb-3"
              v-for="takeaway in takeaway" v-bind:key="takeaway"
            >
              <p class="syne text-lg mb-1">{{takeaway.name}}</p>
              <p class="open text-sm">Abierto de {{takeaway.opening_time}} - {{takeaway.closing_time}}</p>
              <p class="open text-sm">
                {{takeaway.address}}
              </p>
            </div>
          </div>
        </div>
        <div id="map" class="lg:col-span-1">
          <div class="col-span-3 mt-12 hidden md:block">
            <img src="@/assets/landing/fakemap.svg" class="w-full h-full" />
          </div>
        </div>
      </div>
      <div id="section-4" class="">
        <div class="carousel relative shadow-2xl bg-white pb-10">
          <div class="relative ">
            <img
              src="@/assets/landing/figure.svg"
              id="figure"
              class="invisible md:visible"
            />
            <img
              src="@/assets/landing/figure2.svg"
              id="figure2"
              class="invisible md:visible"
            />
            <img
              src="@/assets/landing/ketchup.svg"
              id="figure3"
              class="invisible lg:visible"
            />
          </div>
          <div class="carousel-inner relative overflow-hidden w-full ">
            <!--Slide 1-->
            <input
              class="carousel-open"
              type="radio"
              id="carousel-1"
              name="carousel"
              aria-hidden="true"
              hidden=""
              checked="checked"
            />
            <div class="carousel-item absolute opacity-0">
              <div class="block h-full w-full text-center">
                <p class="druk-bold text-xl mb-2 md:text-3xl">
                  “El mejor lugar para degustar en familia y amigos!”
                </p>
                <p class="open-gray text-lg md:text-xl md:px-12">
                  Es el mejor lugar al que he venido con mi familia, la comida
                  es rica, sirven rápido y te atienden de la mejor manera.
                </p>
              </div>
            </div>
            <label
              for="carousel-2"
              class="prev control-1 w-10 h-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:bg-white rounded-full hover:bg-white  leading-tight  z-10 bottom-0  left-0 my-auto"
              >‹</label
            >
            <label
              for="carousel-2"
              class="next control-1 w-10 h-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:bg-white rounded-full hover:bg-white  leading-tight  z-10 bottom-0 right-0 my-auto"
              >›</label
            >

            <!--Slide 2-->
            <input
              class="carousel-open"
              type="radio"
              id="carousel-2"
              name="carousel"
              aria-hidden="true"
              hidden=""
            />
            <div class="carousel-item absolute opacity-0">
              <div class="block h-full w-full text-center">
                <p class="druk-bold text-xl mb-2 md:text-3xl">
                  “El mejor lugar para degustar en familia!”
                </p>
                <p class="open-gray text-lg md:text-xl md:px-12">
                  Es el mejor lugar al que he venido con mi familia, sirven
                  rápido y te atienden de la mejor manera.
                </p>
              </div>
            </div>
            <label
              for="carousel-1"
              class="prev control-2 w-10 h-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:bg-white rounded-full hover:bg-white  leading-tight  z-10 bottom-0 left-0 my-auto"
              >‹</label
            >
            <label
              for="carousel-1"
              class="next control-2 w-10 h-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:bg-white rounded-full hover:bg-white  leading-tight  z-10 bottom-0 right-0 my-auto"
              >›</label
            >
          </div>
        </div>
      </div>
      <div id="section-5" class="pt-20 bg-black px-6 md:px-16 text-white">
        <div class="container ">
          <p class="druk-bold text-3.5xl text-center mb-6">
            Cuentanos tu experiencia
          </p>
          <p class="open text-lg md:text-2xl text-center px-2 md:px-10 lg:px-6">
            Don't miss out on our great offers & Receive deals from all our top
            restaurants via e-mail.
          </p>
        </div>
        <form v-on:submit.prevent="hello()" method="post">
          <div class="grid grid-cols-10 lg:mx-32">
            <div class="col-span-10 grid grid-cols-10 lg:col-span-3 lg:mr-6">
              <div
              class="col-span-10 
               grid grid-cols-1 text-white hover:text-yellow-600 mt-4"
            >
              <label for="name" class="text-xs">Nombre y Apellido</label>
              <input
                id="name"
                type="text"
                placeholder="John Doe"
                class="input-opinion bg-black border rounded-md pl-2"
                required
              />
            </div>
            <div
              class="col-span-10 grid grid-cols-1 text-white hover:text-yellow-600 mt-4"
            >
              <label for="email" class="text-xs">Correo electrónico</label>
              <input
                id="email"
                type="email"
                placeholder="j.doe@correo.com"
                class="input-opinion bg-black border rounded-md pl-2"
                required
              />
            </div>
            </div>
            <div
              class="col-span-10 lg:col-span-7 grid grid-cols-1 text-white hover:text-yellow-600 mt-4 lg:ml-6"
            >
              <label for="area" class="text-xs">Mensaje</label>
              <textarea
                name=""
                id="area"
                cols="30"
                rows="5"
                placeholder="El día de ahora mi experiencia fue..."
                class="input-opinion bg-black border rounded-md pl-2"
                required
              ></textarea>
            </div>
            <div class="col-span-10 mt-10 mb-64 flex justify-center lg:justify-end">
              <button
                type="submit"
                class="bg-yellow text-black w-56 h-12 open rounded-md"
              >
                Enviar comentarios
              </button>
            </div>
          </div>
        </form>
      </div>
      <div id="section-6" class="px-4 offset-container lg:grid lg:grid-cols-10">
        <div class="relative h-full lg:col-span-3">
          <img
            src="@/assets/landing/phone.svg"
            class="image-offset responsive-image w-full md:invisible"
          />
          <img
            src="@/assets/landing/phone2.svg"
            class="image-offset2 responsive-image w-full invisible md:visible lg:invisible"
          />
          <img
            src="@/assets/landing/phone3.svg"
            class="image-offset3 invisible lg:visible"
          />
        </div>
        <div class="lg:col-span-7">
          <div class="relative mt-16 md:mt-64">
          <div
            class="relative z-10 leading-9 druk-bold text-3xl text-center md:text-3.5xl"
          >
            Obten más beneficios
          </div>
          <div
            class="relative z-10 leading-9 druk-bold text-3xl text-center md:text-3.5xl"
          >
            Descarga nuestra App
          </div>
          <img
            src="@/assets/landing/bg2_text.svg"
            class="absolute inset-x-0 bottom-0 z-0 w-full px-4 md:h-8"
          />
        </div>
        <div class="relative">
          <div class="relative grid grid-cols-2 mt-20">
            <div
              class="relative col-span-2 md:col-span-1 px-4  grid justify-items-center mb-16"
            >
              <img src="@/assets/landing/01.svg" class="mb-2" />
              <img
                src="@/assets/landing/arrow-left.svg"
                class="absolute invisible md:visible"
              />
              <p class="text-center open-bold text-xl mb-6">
                Solicita rápido
              </p>
              <p class="text-center text-lg open">
                Curabitur in eleifend turpis, id vehicula odio. Donec pulvinar
                tellus eget magna aliquet ultricies.
              </p>
            </div>
            <div
              class="col-span-2 md:col-span-1 px-4  grid justify-items-center mb-16"
            >
              <img src="@/assets/landing/02.svg" class="mb-2" />
              <img
                src="@/assets/landing/arrow-right.svg"
                class="absolute invisible md:visible right-0 pr-12"
              />
              <p class="text-center open-bold text-xl mb-6">
                Fácil de Usar
              </p>
              <p class="text-center text-lg open">
                Orci varius natoque penatibus et magnis dis parturient montes,
                nascetur ridiculus mus.
              </p>
            </div>
            <div class="col-span-2 px-4  grid justify-items-center mb-16">
              <img src="@/assets/landing/03.svg" class="mb-2" />
              <p class="text-center open-bold text-xl mb-6">
                Promociones especiales
              </p>
              <p class="text-center text-lg open md:mx-48">
                Curabitur in eleifend turpis, id vehicula odio. Donec pulvinar
                tellus eget magna aliquet ultricies.
              </p>
            </div>
          </div>
          <div class="absolute invisible md:visible">
            <img
              src="@/assets/landing/bg2_text.svg"
              class="absolute inset-x-0 bottom-0 z-0 w-full px-4 md:h-8"
            />
          </div>
        </div>
        </div>
      </div>
      <footer class="mt-32">
        <div class="grid grid-cols-3 mt-8 mx-4 pb-2 footer-yellow">
          <div class="col-span-3 h-6 flex justify-center">
            <img src="@/assets/landing/foodies.svg" class="" />
          </div>
          <div class="col-span-3 h-8 row flex justify-center my-4">
            <img
              src="@/assets/landing/app-store.svg"
              class="h-full float-left mr-2"
            />
            <img src="@/assets/landing/google.svg" class="h-full float-left" />
          </div>
        </div>
        <div class="grid grid-cols-9 mt-8 mx-4 pb-2 mb-8">
          <div
            class="col-span-9 md:col-span-3 lg:col-span-1 open-gray text-center mb-4"
          >
            Conoce nuestras sucursales
          </div>
          <div
            class="col-span-9 md:col-span-3 lg:col-span-1 open-gray text-center mb-4"
          >
            Acerca de
          </div>
          <div
            class="col-span-9 md:col-span-3 lg:col-span-1 open-gray text-center mb-4"
          >
            Conoce nuestras sucursales
          </div>
          <div
            class="col-span-9 md:col-span-3 lg:col-span-1 open-gray text-center mb-4"
          >
            ¿Qué hablan de nosotros?
          </div>
          <div
            class="col-span-9 md:col-span-3 lg:col-span-1 open-gray text-center mb-4"
          >
            Contáctanos
          </div>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
const axios = require("axios");
export default {
  data: () => ({
    Menu: true,
    takeaway: [],
    delivery: [],
    selected:true,
  }),
  created() {
    this.GetTakeaway();
    this.GetDelivery();
    this.PostComments();
  },
  methods: {
    GetTakeaway: function() {
      axios
        .get("https://api.elaniin.dev/api/locations?type=takeaway")
        .then((response) => {
          this.takeaway = response.data.data.map((location) => location);
        })
        .catch(function(error) {
          // handle error
          console.log(error);
        });
    },
    GetDelivery: function() {
      axios
        .get("https://api.elaniin.dev/api/locations?type=delivery")
        .then((response) => {
          this.delivery = response.data.data.map((location) => location);
        })
        .catch(function(error) {
          // handle error
          console.log(error);
        });
    },
    PostComments: function(name,email,comment) {
      axios
        .post("https://api.elaniin.dev/api/contact", {
          "name": name,
          "email": email,
          "message":comment
        })
        .then(function(response) {
          console.log(response);
        })
        .catch(function(error) {
          console.log(error);
        });
    },
  },
};
</script>
<style>
#figure {
  position: absolute;
  top: -20;
}
#figure2 {
  position: absolute;
  top: 20vh;
  right: 0;
}
#figure3 {
  position: absolute;
  top: -1vh;
  right: 0;
}
.ribon {
  bottom: -8em;
}
.offset-container {
  padding-top: 80px;
}
.image-offset {
  position: absolute;
  z-index: 1;
  bottom: -13em;
}
.image-offset2 {
  position: absolute;
  z-index: 1;
  bottom: -30em;
}
.image-offset3 {
  position: absolute;
  overflow: visible;
  width: 100%;
  bottom: -18em;
  right: -5em;
  object-fit:unset;
}

.responsive-image {
  max-width: 100%;
  height: auto;
}
.bg-yellow {
  background: rgba(255, 214, 0, 1);
}
.text-yellow {
  color: rgba(255, 214, 0, 1);
}
.footer-yellow {
  border-bottom-color: rgba(255, 214, 0, 1);
  border-bottom-width: 1px;
}
.druk-bold {
  font-family: "Druk", Helvetica, Arial;
  font-style: normal;
  font-weight: 700;

}
.open {
  font-family: Open Sans;
  font-style: normal;
  font-weight: 400;
  line-height: 22px;
}
.open-bold {
  font-family: Open Sans;
  font-style: normal;
  font-weight: 700;
  line-height: 22px;
}
.open-gray {
  font-family: Open Sans;
  font-style: normal;
  font-weight: 400;
  line-height: 22px;

  color: rgba(0, 0, 0, 0.4);
}
.syne {
  font-family: Syne;
  font-style: normal;
  font-weight: bold;
}
.food-img {
  display: block;
  height: 565px !important;
}
.rounded-b-large {
  border-bottom-right-radius: 30px;
  border-bottom-left-radius: 30px;
}
.input::placeholder {
  font-family: Open Sans;
  font-style: normal;
  font-weight: 400;
  line-height: 22px;

  color: rgba(0, 0, 0, 0.4);
}
.input-opinion::placeholder {
  font-family: Open Sans;
  font-style: normal;
  font-weight: 400;
  line-height: 22px;

  color: rgba(89, 89, 89, 1);
}

.directions {
  height: 102px;
}
.prev {
  margin-left: 30%;
}
.next {
  margin-right: 30%;
}
.carousel-open:checked + .carousel-item {
  position: static;
  opacity: 100;
}
.carousel-item {
  height: 60vh;
  padding-top: 20vh;
  padding-left: 5%;
  padding-right: 5%;
}
#carousel-1:checked ~ .control-1,
#carousel-2:checked ~ .control-2 {
  display: block;
}
.carousel-indicators {
  list-style: none;
  margin: 0;
  padding: 0;
  position: absolute;
  bottom: 2%;
  left: 0;
  right: 0;
  text-align: center;
  z-index: 10;
}
</style>
