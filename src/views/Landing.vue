<template>
  <div class="relative">
    <div
      id="nav"
      class="absolute w-full z-40 pt-12 px-4 md:pt-8 md:px-8 lg:pt-16 lg-px-12"
    >
      <div class="foodies font-bold float-left">Foodies</div>
      <img src="@/assets/landing/menu.svg" class="float-right w-auto pt-1" />
    </div>
    <div id="background" class="absolute z-0 w-full">
      <img
        src="@/assets/landing/vector.svg"
        class="float-right w-full pl-1 md:w-7/12 lg:w-6.5/12"
      />
    </div>
    <div id="content" class="absolute z-10 w-full h-full pt-32 lg:pt-40">
      <!-- <div class="bg-black mx-auto h-screen w-1 z-10"></div> -->
      <div id="section-1" class="container  mx-auto pl-8 pr-2 ">
        <div class="container w-full md:w-1/2">
          <img
            src="@/assets/landing/burger.svg"
            class="w-bw md:w-7/12 lg:w-4/12"
          />
        </div>
        <div class="container pt-10 w-full md:w-1/2">
          <div class="relative">
            <div
              class="relative z-10 leading-9 druk-bold text-3.5xl sm:text-4.5xl md:text-6xl"
            >
              Un nuevo sabor esta en la ciudad
            </div>
            <img
              src="@/assets/landing/bg_text.svg"
              class="absolute bottom-0 left-0 z-0 w-9/12"
            />
          </div>
          <div class="open mt-8 mr-12  text-l md:text-4.5xl lg:text-6.5xl">
            Estamos a punto de descubrir un mundo lleno de sabores y de
            emociones inigualables.
          </div>
          <div class="syne mt-8 text-2xl md:text-4.5xl lg:text-6.5xl">
            <p class="block float-left">Encuentranos</p>
            <img src="@/assets/landing/arrow.svg" class="float-left mt-2" />
          </div>
        </div>
      </div>
      <div id="section-2" class="mt-24 overflow-hidden">
        <div class="relative inline-block container ">
          <img src="@/assets/landing/people.svg" class="max-w-none " />
          <div
            class="absolute bottom-0 right-0 druk-bold text-white mr-2 ml-4 text-right leading-9 text-4.5xl sm:text-4.5xl md:text-6xl"
          >
            <p class="inline">La comida es</p>
            <p class="inline text-yellow-600">nuestro arte</p>
          </div>
        </div>
        <div class="container">
          <div class="syne">
            ¿Quién es Foodies?
          </div>
          <div class="open">
            Elit irure ad nulla id elit laborum nostrud mollit irure. Velit
            reprehenderit sunt nulla enim aliquip duis tempor est culpa fugiat
            consequat culpa consectetur Lorem. Reprehenderit dolore culpa irure
            eiusmod minim occaecat et id minim ullamco.
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.druk-bold {
  font-family: "Druk", Helvetica, Arial;
  font-style: normal;
  font-weight: 700;
  letter-spacing: 0em;
}
.open {
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
.foodies {
  font-family: "Druk";
  font-style: normal;
  font-weight: bold;
  font-size: 27px;
  line-height: 27px;
}
.food-img {
  display: block;
  height: 565px !important;
}
</style>
