<script>
export default {
  data: () => ({
    tab: null,
    tab2: null
  })
}
</script>
<template>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=League+Spartan:wght@100..900&family=Roboto:wght@400;700&display=swap"
    rel="stylesheet"
  />
  <div class="edHome">
    <header>
      <v-container>
        <v-row>
          <v-col>
            <img src="../img/logo.png" class="logo" alt="logo" />
          </v-col>
          <v-col class="text-end">
            <v-btn flat class="rounded-pill border px-10 text-capitalize">Login</v-btn>
          </v-col>
        </v-row>
      </v-container>
    </header>

    <v-container>
      <v-row>
        <v-col md="6">
          <p class="text-h6 mb-4">De digitale onderwijsassistent</p>
          <h1 class="mb-8 text-h3 mainHeading">Bespaar tijd met jouw onderwijsassistent</h1>
          <p class="mb-3 text-subtitle-1">
            Docenten van alle onderwijsniveaus gebruiken online assistenten om sneller te kunnen
            werken
          </p>
          <v-row>
            <v-col>
              <v-btn class="mb-1 btn rounded-pill text-h6">Gebruik Gratis!</v-btn>
              <div class="semibold textGray">Geen credit card nodig.</div>
            </v-col>
            <v-col class="text-end">
              <img src="../img/Image1.png" alt="image" class="Image1" />
            </v-col>
          </v-row>
        </v-col>
        <v-col md="6" class="ps-sm-0 ps-md-0 ps-lg-0 ps-xl-0">
          <v-card class="pa-4 rounded-xl topCard">
            <v-tabs v-model="tab" align-tabs="center">
              <v-tab value="one">Mbo</v-tab>
              <v-tab value="two">Hbo</v-tab>
              <v-tab value="three">Wo</v-tab>
            </v-tabs>
            <v-window v-model="tab">
              <v-window-item value="one">
                <h5 class="mt-1 ms-6 text-h5 mb-5">Omar - mbo<br />onderwijsassistent</h5>
                <v-form ref="form">
                  <label>Skills van Omar</label>
                  <div class="mt-2">
                    <label class="radioInput">
                      <input type="radio" name="radio-group" value="one" /> Opbouwende feedback
                    </label>
                    <label class="radioInput">
                      <input type="radio" name="radio-group" value="one" /> Taalgebruik ondersteunen
                    </label>
                    <label class="radioInput">
                      <input type="radio" name="radio-group" value="one" /> Taxonomie van Bloem
                    </label>
                  </div>

                  <div class="mt-3">
                    <label>Upload opdracht student (pdf)</label>
                    <label class="fileUpload">
                      <input type="file" placeholder="Upload Box" />
                      Upload box
                    </label>
                  </div>

                  <div class="mt-3">
                    <label>Belangrijkste Leerdoel</label>
                    <textarea
                      class="w-100 border"
                      rows="4"
                      placeholder="Geef aan wat het belangrijkste leerdoel is dat de student leert uit de opdracht Bijvoorbeeld het vergelijken van Nederlandse taal met Engelsi"
                    ></textarea>
                  </div>
                  <v-btn class="btn rounded-pill shadow-none mt-3">Creéer feedback</v-btn>
                </v-form>
              </v-window-item>
              <v-window-item value="two">
                <h5 class="mt-1 ms-6 text-h5 mb-5">Omar - mbo<br />onderwijsassistent</h5>
                <v-form ref="form">
                  <label>Skills van Omar</label>
                  <div class="mt-2">
                    <label class="radioInput">
                      <input type="radio" name="radio-group" value="one" /> Opbouwende feedback
                    </label>
                    <label class="radioInput">
                      <input type="radio" name="radio-group" value="one" /> Taalgebruik ondersteunen
                    </label>
                    <label class="radioInput">
                      <input type="radio" name="radio-group" value="one" /> Taxonomie van Bloem
                    </label>
                  </div>

                  <div class="mt-3">
                    <label>Upload opdracht student (pdf)</label>
                    <label class="fileUpload">
                      <input type="file" placeholder="Upload Box" />
                      Upload box
                    </label>
                  </div>

                  <div class="mt-3">
                    <label>Belangrijkste Leerdoel</label>
                    <textarea
                      class="w-100 border"
                      rows="4"
                      placeholder="Geef aan wat het belangrijkste leerdoel is dat de student leert uit de opdracht Bijvoorbeeld het vergelijken van Nederlandse taal met Engelsi"
                    ></textarea>
                  </div>
                  <v-btn class="btn rounded-pill shadow-none mt-3">Creéer feedback</v-btn>
                </v-form>
              </v-window-item>
              <v-window-item value="three">
                <h5 class="mt-1 ms-6 text-h5 mb-5">Omar - mbo<br />onderwijsassistent</h5>
                <v-form ref="form">
                  <label>Skills van Omar</label>
                  <div class="mt-2">
                    <label class="radioInput">
                      <input type="radio" name="radio-group" value="one" /> Opbouwende feedback
                    </label>
                    <label class="radioInput">
                      <input type="radio" name="radio-group" value="one" /> Taalgebruik ondersteunen
                    </label>
                    <label class="radioInput">
                      <input type="radio" name="radio-group" value="one" /> Taxonomie van Bloem
                    </label>
                  </div>

                  <div class="mt-3">
                    <label>Upload opdracht student (pdf)</label>
                    <label class="fileUpload">
                      <input type="file" placeholder="Upload Box" />
                      Upload box
                    </label>
                  </div>

                  <div class="mt-3">
                    <label>Belangrijkste Leerdoel</label>
                    <textarea
                      class="w-100 border"
                      rows="4"
                      placeholder="Geef aan wat het belangrijkste leerdoel is dat de student leert uit de opdracht Bijvoorbeeld het vergelijken van Nederlandse taal met Engelsi"
                    ></textarea>
                  </div>
                  <v-btn class="btn rounded-pill shadow-none mt-3">Creéer feedback</v-btn>
                </v-form>
              </v-window-item>
            </v-window>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <v-container>
      <v-row>
        <v-col md="6" class="text-end">
          <h3 class="text-h4 mt-2">Ik ben docent op het..</h3>
        </v-col>
        <v-col md="6">
          <v-tabs v-model="tab2" align-tabs="center" class="d-inline-block m-auto">
            <v-tab value="Mbo">Mbo</v-tab>
            <v-tab value="Hbo">Hbo</v-tab>
            <v-tab value="Wo">Wo</v-tab>
          </v-tabs>
        </v-col>
      </v-row>
    </v-container>
    <v-window v-model="tab2">
      <v-window-item value="Mbo">
        <v-container>
          <v-row>
            <v-col sm="7">
              <h4 class="text-h4 mb-3">Ontmoet onderwijsassistent Omar</h4>
              <p class="mb-6" style="line-height: 1">
                <small class="font-weight-medium text-subtitle-1"
                  >Hallo, mijn naam is Omar. 1k ben de assistent die je altijd al hebt gewild,<br />
                  maar nog nooit hebt kunnen hebben tot nu.</small
                >
              </p>
              <v-btn class="btn rounded-0 cShadow">Leer meer over mij!</v-btn>
            </v-col>
            <v-col md="5" class="text-end">
              <img src="../img/Image2.png" alt="image" class="Image2" />
            </v-col>
          </v-row>
          <v-row class="">
            <v-col sm="4">
              <div class="cCard">
                <img src="../img/heart.svg" />
                <h2>96%</h2>
                <p>Mbo docenten besparen tijd met een Al assistent</p>
              </div>
            </v-col>
            <v-col md="4">
              <div class="cCard">
                <img src="../img/people.svg" />
                <h2>1.000+</h2>
                <p>Mbo docenten gebruiken dagelijks een AI assistent</p>
              </div>
            </v-col>
            <v-col md="4">
              <div class="cCard">
                <img src="../img/feedback.svg" />
                <h2>50.000+</h2>
                <p>Geeft een Eduface assistent feedback per maand</p>
              </div>
            </v-col>
          </v-row>
          <v-row class="mt-8">
            <v-col cols="12" sm="6" class="text-end">
              <img src="../img/Image3.png" class="Image3" />
            </v-col>
            <v-col cols="12" sm="6" class="mt-sm-16 laatMij">
              <div class="mx-auto" style="max-width: 550px">
                <h3 class="mt-sm-12 mt-md-14 mt-lg-16 text-h6 mb-6">
                  Laat mij jou ondersteunen bij jouw onderwijstaken! Dit is wat ik kan:
                </h3>
                <p>
                  <img src="../img/file.svg" class="me-1" /> Ik kan formatieve feedback geven op de
                  opdrachten van jouw studenten
                </p>
                <p>
                  <img src="../img/box.svg" class="me-1" /> Ik kan onbeperkte veel oefenvragen maken
                  in jouw eigen digitale leeromgeving.
                </p>
                <p>
                  <img src="../img/people.svg" class="me-1" /> Ik ben helemaal AVG proof gebouwd en
                  ik sla geen informatie op!
                </p>
                <div class="cCard uploadBox">
                  <div><img src="../img/upload.svg" /></div>
                  Laat mij feedback geven op het werk <br />van jouw studenten
                </div>
              </div>
            </v-col>
          </v-row>
          <v-row class="">
            <v-col cols="12" sm="5">
              <div class="reviewLeft">
                <v-row>
                  <v-col class="txt">
                    Tamara Metz - software development docent
                    <div class="mt-4 txt">MboRijnIand</div>
                  </v-col>
                  <v-col class="text-center">
                    <img src="../img/Image4.png" />
                  </v-col>
                </v-row>
              </div>
            </v-col>
            <v-col cols="12" sm="7" class="reviewRight">
              <h5 class="text-h5 font-weight-bold">
                "Omar heeft mij geholpen om meer dan IO uur per week te besparen op het maken van
                oefenmateriaal en op het nakijken en voorzien van feedback voor mijn studenten'
              </h5>
              <div class="starts">
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
              </div>
            </v-col>
          </v-row>
        </v-container>
        <div class="greenBg">
          <v-container class="py-8">
            <v-row>
              <v-col cols="12" sm="6"><img src="../img/Image5.png" /></v-col>
              <v-col cols="12" sm="6">
                <div class="ps-0 ps-sm-4 ps-md-6 ps-lg-8">
                  <h4 class="text-h4 font-weight-bold mb-4">
                    Ik kan niet wachten om samen te werken!
                  </h4>
                  <p class="mb-6 text-subtitle-1">
                    Ik heb goed nieuws! 1k sla geen informatie op, want ik benvolledig AVG proof
                    gebouwd.
                  </p>
                  <v-btn class="btn rounded-0">Samenwerken met Omar</v-btn>
                </div>
              </v-col>
            </v-row>
          </v-container>
        </div>
      </v-window-item>
      <v-window-item value="Hbo">
        <v-container>
          <v-row>
            <v-col sm="7">
              <h4 class="text-h4 mb-3">Ontmoet onderwijsassistent Omar</h4>
              <p class="mb-6" style="line-height: 1">
                <small class="font-weight-medium text-subtitle-1"
                  >Hallo, mijn naam is Omar. 1k ben de assistent die je altijd al hebt gewild,<br />
                  maar nog nooit hebt kunnen hebben tot nu.</small
                >
              </p>
              <v-btn class="btn rounded-0 cShadow">Leer meer over mij!</v-btn>
            </v-col>
            <v-col md="5" class="text-end">
              <img src="../img/Image2.png" alt="image" class="Image2" />
            </v-col>
          </v-row>
          <v-row class="">
            <v-col sm="4">
              <div class="cCard">
                <img src="../img/heart.svg" />
                <h2>96%</h2>
                <p>Mbo docenten besparen tijd met een Al assistent</p>
              </div>
            </v-col>
            <v-col md="4">
              <div class="cCard">
                <img src="../img/people.svg" />
                <h2>1.000+</h2>
                <p>Mbo docenten gebruiken dagelijks een AI assistent</p>
              </div>
            </v-col>
            <v-col md="4">
              <div class="cCard">
                <img src="../img/feedback.svg" />
                <h2>50.000+</h2>
                <p>Geeft een Eduface assistent feedback per maand</p>
              </div>
            </v-col>
          </v-row>
          <v-row class="mt-8">
            <v-col cols="12" sm="6" class="text-end">
              <img src="../img/Image3.png" class="Image3" />
            </v-col>
            <v-col cols="12" sm="6" class="mt-sm-16 laatMij">
              <div class="mx-auto" style="max-width: 550px">
                <h3 class="mt-sm-12 mt-md-14 mt-lg-16 text-h6 mb-6">
                  Laat mij jou ondersteunen bij jouw onderwijstaken! Dit is wat ik kan:
                </h3>
                <p>
                  <img src="../img/file.svg" class="me-1" /> Ik kan formatieve feedback geven op de
                  opdrachten van jouw studenten
                </p>
                <p>
                  <img src="../img/box.svg" class="me-1" /> Ik kan onbeperkte veel oefenvragen maken
                  in jouw eigen digitale leeromgeving.
                </p>
                <p>
                  <img src="../img/people.svg" class="me-1" /> Ik ben helemaal AVG proof gebouwd en
                  ik sla geen informatie op!
                </p>
                <div class="cCard uploadBox">
                  <div><img src="../img/upload.svg" /></div>
                  Laat mij feedback geven op het werk <br />van jouw studenten
                </div>
              </div>
            </v-col>
          </v-row>
          <v-row class="">
            <v-col cols="12" sm="5">
              <div class="reviewLeft">
                <v-row>
                  <v-col class="txt">
                    Tamara Metz - software development docent
                    <div class="mt-4 txt">MboRijnIand</div>
                  </v-col>
                  <v-col class="text-center">
                    <img src="../img/Image4.png" />
                  </v-col>
                </v-row>
              </div>
            </v-col>
            <v-col cols="12" sm="7" class="reviewRight">
              <h5 class="text-h5 font-weight-bold">
                "Omar heeft mij geholpen om meer dan IO uur per week te besparen op het maken van
                oefenmateriaal en op het nakijken en voorzien van feedback voor mijn studenten'
              </h5>
              <div class="starts">
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
              </div>
            </v-col>
          </v-row>
        </v-container>
        <div class="greenBg">
          <v-container class="py-8">
            <v-row>
              <v-col cols="12" sm="6"><img src="../img/Image5.png" /></v-col>
              <v-col cols="12" sm="6">
                <div class="ps-0 ps-sm-4 ps-md-6 ps-lg-8">
                  <h4 class="text-h4 font-weight-bold mb-4">
                    Ik kan niet wachten om samen te werken!
                  </h4>
                  <p class="mb-6 text-subtitle-1">
                    Ik heb goed nieuws! 1k sla geen informatie op, want ik benvolledig AVG proof
                    gebouwd.
                  </p>
                  <v-btn class="btn rounded-0">Samenwerken met Omar</v-btn>
                </div>
              </v-col>
            </v-row>
          </v-container>
        </div>
      </v-window-item>
      <v-window-item value="Wo">
        <v-container>
          <v-row>
            <v-col sm="7">
              <h4 class="text-h4 mb-3">Ontmoet onderwijsassistent Omar</h4>
              <p class="mb-6" style="line-height: 1">
                <small class="font-weight-medium text-subtitle-1"
                  >Hallo, mijn naam is Omar. 1k ben de assistent die je altijd al hebt gewild,<br />
                  maar nog nooit hebt kunnen hebben tot nu.</small
                >
              </p>
              <v-btn class="btn rounded-0 cShadow">Leer meer over mij!</v-btn>
            </v-col>
            <v-col md="5" class="text-end">
              <img src="../img/Image2.png" alt="image" class="Image2" />
            </v-col>
          </v-row>
          <v-row class="">
            <v-col sm="4">
              <div class="cCard">
                <img src="../img/heart.svg" />
                <h2>96%</h2>
                <p>Mbo docenten besparen tijd met een Al assistent</p>
              </div>
            </v-col>
            <v-col md="4">
              <div class="cCard">
                <img src="../img/people.svg" />
                <h2>1.000+</h2>
                <p>Mbo docenten gebruiken dagelijks een AI assistent</p>
              </div>
            </v-col>
            <v-col md="4">
              <div class="cCard">
                <img src="../img/feedback.svg" />
                <h2>50.000+</h2>
                <p>Geeft een Eduface assistent feedback per maand</p>
              </div>
            </v-col>
          </v-row>
          <v-row class="mt-8">
            <v-col cols="12" sm="6" class="text-end">
              <img src="../img/Image3.png" class="Image3" />
            </v-col>
            <v-col cols="12" sm="6" class="mt-sm-16 laatMij">
              <div class="mx-auto" style="max-width: 550px">
                <h3 class="mt-sm-12 mt-md-14 mt-lg-16 text-h6 mb-6">
                  Laat mij jou ondersteunen bij jouw onderwijstaken! Dit is wat ik kan:
                </h3>
                <p>
                  <img src="../img/file.svg" class="me-1" /> Ik kan formatieve feedback geven op de
                  opdrachten van jouw studenten
                </p>
                <p>
                  <img src="../img/box.svg" class="me-1" /> Ik kan onbeperkte veel oefenvragen maken
                  in jouw eigen digitale leeromgeving.
                </p>
                <p>
                  <img src="../img/people.svg" class="me-1" /> Ik ben helemaal AVG proof gebouwd en
                  ik sla geen informatie op!
                </p>
                <div class="cCard uploadBox">
                  <div><img src="../img/upload.svg" /></div>
                  Laat mij feedback geven op het werk <br />van jouw studenten
                </div>
              </div>
            </v-col>
          </v-row>
          <v-row class="">
            <v-col cols="12" sm="5">
              <div class="reviewLeft">
                <v-row>
                  <v-col class="txt">
                    Tamara Metz - software development docent
                    <div class="mt-4 txt">MboRijnIand</div>
                  </v-col>
                  <v-col class="text-center">
                    <img src="../img/Image4.png" />
                  </v-col>
                </v-row>
              </div>
            </v-col>
            <v-col cols="12" sm="7" class="reviewRight">
              <h5 class="text-h5 font-weight-bold">
                "Omar heeft mij geholpen om meer dan IO uur per week te besparen op het maken van
                oefenmateriaal en op het nakijken en voorzien van feedback voor mijn studenten'
              </h5>
              <div class="starts">
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
                <img src="../img/star.svg" />
              </div>
            </v-col>
          </v-row>
        </v-container>
        <div class="greenBg">
          <v-container class="py-8">
            <v-row>
              <v-col cols="12" sm="6"><img src="../img/Image5.png" /></v-col>
              <v-col cols="12" sm="6">
                <div class="ps-0 ps-sm-4 ps-md-6 ps-lg-8">
                  <h4 class="text-h4 font-weight-bold mb-4">
                    Ik kan niet wachten om samen te werken!
                  </h4>
                  <p class="mb-6 text-subtitle-1">
                    Ik heb goed nieuws! 1k sla geen informatie op, want ik benvolledig AVG proof
                    gebouwd.
                  </p>
                  <v-btn class="btn rounded-0">Samenwerken met Omar</v-btn>
                </div>
              </v-col>
            </v-row>
          </v-container>
        </div>
      </v-window-item>
    </v-window>
  </div>
</template>

<style scoped>
* {
  font-family: 'League Spartan', sans-serif;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
  color: #414042;
}

@media (min-width: 1920px) {
  .v-container {
    max-width: 1350px;
  }
}
.mainHeading {
  letter-spacing: 2px;
}
.btn {
  background-color: #00e075;
  box-shadow: none;
  font-weight: 600;
  text-transform: capitalize;
  font-size: 16px;
  padding: 15px 25px;
  height: auto !important;
}
.btn:hover {
  box-shadow: none;
}
.semibold {
  font-weight: 600;
}
.textGray {
  color: #8a8a8a;
}

.topCard {
  background-color: #ebebeb;
  border: 1px solid #686868;
  box-shadow: rgba(0, 0, 0, 0.1) 0px 4px 12px !important;
}

.radioInput {
  background: #fff;
  padding: 4px 8px 2px 8px;
  margin-right: 8px;
  margin-bottom: 8px;
  letter-spacing: -0.4px;
  display: inline-block;
  font-size: 14px;
  border-radius: 15px;
}
.radioInput input {
  display: none;
}
.fileUpload {
  display: block;
  cursor: pointer;
  background: #fff;
  color: #adadad;
  padding: 8px 10px;
  border-radius: 15px;
  margin-top: 5px;
}
.fileUpload input {
  display: none;
}
textarea {
  background: #fff;
  border-radius: 15px;
  padding: 8px 10px;
}
textarea::placeholder {
  font-size: 12px;
}
.Image1 {
  max-width: 100%;
  width: 150px;
}
.cShadow {
  box-shadow: #414142 5px 5px 0px !important;
}
.Image2 {
  max-width: 100%;
  width: 230px;
}
.cCard {
  background-color: #f6f2f7;
  padding: 15px 25px;
  border-radius: 8px;
}

.cCard img {
  max-width: 100%;
  width: 25px;
  margin-right: 10px;
}
.cCard h2 {
  font-size: 43px;
  font-weight: 400 !important;
}
.cCard p {
  font-size: 18px;
  font-weight: 700 !important;
}
.Image3 {
  max-width: 100%;
}
.laatMij p {
  font-weight: 600;
  line-height: 1.5;
  margin-bottom: 10px;
}
.laatMij img {
  vertical-align: middle;
}
.uploadBox {
  margin-top: 15px;
  text-align: center;
  font-weight: 700;
  border: 2px solid #8bebad;
}
.uploadBox img {
  width: 50px !important;
}
.reviewLeft {
  box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
  border-radius: 10px;
  padding: 15px 25px;
}
.reviewLeft .txt {
  font-weight: 700;
  font-size: 20px;
}
.reviewLeft img {
  width: 100%;
  max-width: 140px;
}
.reviewRight h3 {
  font-weight: 600;
}
.starts {
  display: inline-block;
  margin-top: 40px;
  border-bottom: 5px solid #000;
}
.starts img {
  width: 50px;
}

.greenBg {
  margin-top: 15px;
  background-color: #bfe3d6;
}
.greenBg img {
  max-width: 100%;
  width: 500px;
}
.greenBg h2 {
  margin-top: 50px;
  font-weight: 600;
}
.greenBg p {
  font-size: 14px;
  line-height: 1;
  margin-bottom: 20px;
}
</style>
