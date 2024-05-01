<script>
export default {
  data: () => ({
    tab: null,
    tab2: null,
    colors: ['primary', 'secondary', 'yellow darken-2', 'red', 'orange'],
    model: 0
  })
}
</script>
<template>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />

  <div class="edHome">
    <header>
      <div class="eContainer">
        <div class="eRow my-2">
          <div class="col">
            <img src="../img/logo.png" class="logo" alt="logo" />
          </div>
          <div class="col text-end">
            <v-btn flat class="rounded-pill border px-10 text-capitalize loginBtn">Login</v-btn>
          </div>
        </div>
      </div>
    </header>

    <div class="eContainer my-4 pb-5">
      <div class="eRow md-my-16">
        <div class="col-md-5">
          <h3 class="text-h4 mt-sm-16 mt-md-16 pt-md-16 font-weight-bold">Al Omar</h3>
          <p class="mt-5 text-h6">
            Hallo, mijn naam is Omar. 1k ben de assistent die je altijd al hebt gewild, maar nog
            nooit hebt kunnen hebben tot nu.
          </p>

          <div class="pt-4 mt-md-16">
            <v-btn class="btn rounded-0 font-weight-bold">Samenwerken met Omar</v-btn>
          </div>
        </div>
        <div class="col-md-7">
          <div class="mt-5 my-md-0 pt-md-4">
            <v-responsive :aspect-ratio="16 / 9" class="video py-5"
              ><iframe
                class="w-100 h-100"
                src="https://app.supademo.com/embed/clvkyla770ut5769d1gnmtpab"
                allow="clipboard-write"
                frameborder="0"
                webkitallowfullscreen="true"
                mozallowfullscreen="true"
                allowfullscreen
              ></iframe>
            </v-responsive>
          </div>
        </div>
      </div>
    </div>

    <div class="eContainer my-4 stappen">
      <h3 class="text-h3 my-6 text-center">Start in 3 stappen</h3>
      <div class="eRow mt-4 mt-lg-0 gCard">
        <div class="col-md-4 my-3">
          <div class="cCard">
            <span class="num">1</span> <img src="../img/star.svg" />
            <h4 class="text-h4">
              Maak een gratis <br />
              accountje aan!
            </h4>
            <div class="hoverShow">
              <v-responsive :aspect-ratio="16 / 9">
                <iframe
                  class="w-100 h-100"
                  src="https://app.supademo.com/embed/clvkyla770ut5769d1gnmtpab"
                  allow="clipboard-write"
                  frameborder="0"
                  webkitallowfullscreen="true"
                  mozallowfullscreen="true"
                  allowfullscreen
                ></iframe>
              </v-responsive>
            </div>
          </div>
        </div>
        <div class="col-md-4 my-3">
          <div class="cCard">
            <span class="num">2</span> <img src="../img/star.svg" />
            <h4 class="text-h4">Upload jouw eerste beoordelingsformulier of rubriek</h4>
            <div class="hoverShow">
              <v-responsive :aspect-ratio="16 / 9">
                <iframe
                  class="w-100 h-100"
                  src="https://app.supademo.com/embed/clvkyla770ut5769d1gnmtpab"
                  allow="clipboard-write"
                  frameborder="0"
                  webkitallowfullscreen="true"
                  mozallowfullscreen="true"
                  allowfullscreen
                ></iframe>
              </v-responsive>
            </div>
          </div>
        </div>
        <div class="col-md-4 my-3">
          <div class="cCard">
            <span class="num">3</span> <img src="../img/star.svg" />
            <h4 class="text-h4">
              Upload de opdrachten van jouw studenten en zet mij aan het werk!
            </h4>
            <div class="hoverShow">
              <v-responsive :aspect-ratio="16 / 9">
                <iframe
                  class="w-100 h-100"
                  src="https://app.supademo.com/embed/clvkyla770ut5769d1gnmtpab"
                  allow="clipboard-write"
                  frameborder="0"
                  webkitallowfullscreen="true"
                  mozallowfullscreen="true"
                  allowfullscreen
                ></iframe>
              </v-responsive>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="mt-16">
      <div class="eContainer my-4">
        <h3 class="text-h3 my-12 text-center">De reden van mijn bestaan</h3>
      </div>
      <v-carousel class="carousel" v-model="model" direction="vertical">
        <v-carousel-item>
          <div class="eContainer">
            <div class="eRow">
              <div class="col-md-6 imgDiv">
                <div class="text-end pr-12">
                  <img src="../img/Image1.png" />
                </div>
              </div>
              <div class="col-md-6">
                <div class="cCard p-5 text-h5">
                  Gemiddeld werken docenten meer dan <span class="textGreen">10 uur</span> per week
                  over en <span class="textGreen">96%</span> van de docenten geven aan dat ze de
                  wekelijkse taken niet afkrijgen.
                </div>
              </div>
            </div>
          </div>
        </v-carousel-item>
        <v-carousel-item v-for="i in 5" :key="i">
          <div class="eContainer">
            <div class="eRow">
              <div class="col-md-6 imgDiv">
                <div class="text-end pr-12">
                  <img src="../img/Image2.png" />
                </div>
              </div>
              <div class="col-md-6">
                <div class="cCard p-5 text-h5">
                  Gemiddeld werken docenten meer dan <span class="textGreen">10 uur</span> per week
                  over en <span class="textGreen">96%</span> van de docenten geven aan dat ze de
                  wekelijkse taken niet afkrijgen.
                </div>
              </div>
            </div>
          </div>
        </v-carousel-item>
      </v-carousel>
    </div>
  </div>
</template>

<style>
.v-window__left,
.v-window__right {
  display: none !important;
}
.v-carousel__controls {
  background: #eaeaea !important;
  height: 3px !important;
  width: 300px !important;
  top: 150px !important;
  left: calc(50% - 180px) !important;
  transform: rotate(90deg);
}
.v-carousel__controls .v-btn {
  background: #eaeaea;
  width: 15px !important;
  height: 15px !important;
}
.v-carousel__controls .v-btn.v-btn--active {
  background: #052333;
}
@media (max-width: 767px) {
  .v-carousel__controls {
    left: calc(0% - 130px) !important;
  }
  .carousel .imgDiv {
    display: none;
  }
  .carousel .cCard {
    margin-left: 25px;
  }
}
</style>

<style scoped>
@import '../assets/grid.css';
.carousel img {
  max-width: 100%;
}
.video {
  background-image: url(../img/bg1.png);
  background-size: contain;
  background-position: center;
}

.num {
  font-size: 28px;
  display: inline-block;
  color: #bdbec0;
  font-weight: 700;
}
.gCard img {
  vertical-align: middle;
  margin-left: 5px;
}
.stappen .cCard {
  position: relative;
  height: 260px;
}
.stappen .cCard:hover {
  height: fit-content;
}
.hoverShow {
  display: none;
  margin-top: 15px;
}
.stappen .cCard:hover .hoverShow {
  display: block;
}
</style>
