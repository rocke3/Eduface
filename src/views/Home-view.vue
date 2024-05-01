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

    <div class="eContainer mt-4">
      <div class="eRow">
        <div class="col-lg-6 mt-12">
          <h1 class="mb-8 text-h5 text-sm-h4 text-md-h3 mainHeading">
            Geef opdrachten en feedback met jouw
            <span class="textGreen">AI Onderwijsassistent</span>
          </h1>
          <p class="mb-14" style="font-size: 19px">
            Docenten van alle onderwijsniveaus gebruiken geautomatiseerde
            <span class="textGreen">assistenten</span> om sneller te kunnen werken
          </p>
          <div class="eRow">
            <div class="col-md-6">
              <v-btn class="mb-4 btn rounded-pill text-h6">Bekijk voorbeeld</v-btn>
              <div class="semibold textGreen mb-3">Geen betaalgegevens nodig</div>
              <div class="semibold textGreen">100% AVG en onderwijsproof</div>
            </div>
            <div class="col-md-6 text-center text-lg-end">
              <img src="../img/Image1.png" alt="image" class="Image1" />
            </div>
          </div>
        </div>
        <div class="col-lg-6">
          <v-card class="pa-4 rounded-xl topCard">
            <v-tabs v-model="tab" align-tabs="center">
              <v-tab value="one">Mbo</v-tab>
              <v-tab value="two">Hbo</v-tab>
              <v-tab value="three">Wo</v-tab>
            </v-tabs>
            <v-window v-model="tab">
              <v-window-item value="one">
                <h4 class="mt-2 ms-6 text-h4 mb-8">Omar - Al mbo <br />onderwijsassistent</h4>
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

                  <div class="mt-4">
                    <label>Upload opdracht student (pdf)</label>
                    <label class="fileUpload">
                      <input type="file" placeholder="Upload Box" />
                      Upload box
                    </label>
                  </div>

                  <div class="mt-4">
                    <label>Belangrijkste Leerdoel</label>
                    <textarea
                      class="w-100 border"
                      eRows="4"
                      placeholder="Geef aan wat het belangrijkste leerdoel is dat de student leert uit de opdracht Bijvoorbeeld het vergelijken van Nederlandse taal met Engelsi"
                    ></textarea>
                  </div>
                  <div class="mt-5">
                    <v-btn class="btn rounded-pill shadow-none">Creéer feedback</v-btn>
                  </div>
                </v-form>
              </v-window-item>
              <v-window-item value="two">
                <h4 class="mt-2 ms-6 text-h4 mb-8">Omar - Al mbo <br />onderwijsassistent</h4>
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

                  <div class="mt-4">
                    <label>Upload opdracht student (pdf)</label>
                    <label class="fileUpload">
                      <input type="file" placeholder="Upload Box" />
                      Upload box
                    </label>
                  </div>

                  <div class="mt-4">
                    <label>Belangrijkste Leerdoel</label>
                    <textarea
                      class="w-100 border"
                      eRows="4"
                      placeholder="Geef aan wat het belangrijkste leerdoel is dat de student leert uit de opdracht Bijvoorbeeld het vergelijken van Nederlandse taal met Engelsi"
                    ></textarea>
                  </div>
                  <div class="mt-5">
                    <v-btn class="btn rounded-pill shadow-none">Creéer feedback</v-btn>
                  </div>
                </v-form>
              </v-window-item>
              <v-window-item value="three">
                <h4 class="mt-2 ms-6 text-h4 mb-8">Omar - Al mbo <br />onderwijsassistent</h4>
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

                  <div class="mt-4">
                    <label>Upload opdracht student (pdf)</label>
                    <label class="fileUpload">
                      <input type="file" placeholder="Upload Box" />
                      Upload box
                    </label>
                  </div>

                  <div class="mt-4">
                    <label>Belangrijkste Leerdoel</label>
                    <textarea
                      class="w-100 border"
                      eRows="4"
                      placeholder="Geef aan wat het belangrijkste leerdoel is dat de student leert uit de opdracht Bijvoorbeeld het vergelijken van Nederlandse taal met Engelsi"
                    ></textarea>
                  </div>
                  <div class="mt-5">
                    <v-btn class="btn rounded-pill shadow-none">Creéer feedback</v-btn>
                  </div>
                </v-form>
              </v-window-item>
            </v-window>
          </v-card>
        </div>
      </div>
    </div>

    <div class="eContainer">
      <div class="eRow my-16">
        <div class="col">
          <h3 class="text-h4 mt-16">Wij werken samen met</h3>
          <p class="mt-5 text-subtitle-1">
            Deze partners helpen ons op onze missie om technologie toegankelijk te maken in het
            onderwijs. Geloof jij ook in de kracht van technologie en help jij ons ook?
          </p>
        </div>
        <div class="col text-end">
          <img src="../img/Image6.png" class="logo" alt="logo" />
        </div>
      </div>
    </div>

    <div class="eContainer my-4">
      <div class="eRow">
        <div class="col-md-6 text-center text-md-end mb-4 mb-md-0">
          <h3 class="text-h4 mt-2">Ik ben docent op het..</h3>
        </div>
        <div class="col-md-6 text-center text-md-start mb-4 mb-md-0">
          <v-tabs v-model="tab2" align-tabs="center" class="d-inline-block m-auto">
            <v-tab value="Mbo">Mbo</v-tab>
            <v-tab value="Hbo">Hbo</v-tab>
            <v-tab value="Wo">Wo</v-tab>
          </v-tabs>
        </div>
      </div>
    </div>
    <v-window v-model="tab2">
      <v-window-item value="Mbo">
        <div>
          <div class="eContainer">
            <div class="eRow">
              <div class="col-sm-7">
                <h4 class="text-h4 mb-3">
                  Ontmoet <span class="textGreen">onderwijsassistent</span> Omar
                </h4>
                <p class="mb-6" style="line-height: 1">
                  <small class="font-weight-bold text-subtitle-1"
                    >Hallo, mijn naam is Omar. 1k ben de assistent die je altijd al hebt gewild,<br />
                    maar nog nooit hebt kunnen hebben tot nu.</small
                  >
                </p>
                <v-btn class="btn rounded-0 cShadow">Leer meer over mij!</v-btn>
              </div>
              <div class="col-md-5 text-center text-md-end mt-4 mt-md-0">
                <img src="../img/Image2.png" alt="image" class="Image2" />
              </div>
            </div>
            <div class="eRow mt-4 mt-lg-0 gCard">
              <div class="col-md-4 my-3">
                <div class="cCard">
                  <img src="../img/star.svg" />
                  <h2>96%</h2>
                  <p>Mbo docenten besparen tijd met een Al assistent</p>
                </div>
              </div>
              <div class="col-md-4 my-3">
                <div class="cCard">
                  <img src="../img/star.svg" />
                  <h2>1.000+</h2>
                  <p>Mbo docenten gebruiken dagelijks een AI assistent</p>
                </div>
              </div>
              <div class="col-md-4 my-3">
                <div class="cCard">
                  <img src="../img/star.svg" />
                  <h2>50.000+</h2>
                  <p>Geeft een Eduface assistent feedback per maand</p>
                </div>
              </div>
            </div>
            <div class="mt-8 eRow">
              <div class="col-md-6 text-end">
                <img src="../img/Image3.png" class="Image3" />
              </div>
              <div class="col-md-6 mt-sm-4 mb-8 laatMij">
                <div class="mx-auto" style="max-width: 550px">
                  <h3 class="mt-sm-6 mt-md-14 mt-lg-16 text-h6 mb-6">
                    Laat mij jou ondersteunen bij jouw onderwijstaken! Dit is wat ik kan:
                  </h3>
                  <p>
                    <img src="../img/file.svg" class="me-1" /> Ik kan
                    <span class="textGreen">formatieve feedback</span> geven op de opdrachten van
                    jouw studenten
                  </p>
                  <p>
                    <img src="../img/box.svg" class="me-1" /> Ik kan onbeperkte veel
                    <span class="textGreen">oefenvragen</span> maken in jouw eigen digitale
                    leeromgeving.
                  </p>
                  <p>
                    <img src="../img/people.svg" class="me-1" /> Ik ben helemaal
                    <span class="textGreen">AVG</span> proof gebouwd en ik sla geen informatie op!
                  </p>
                  <div class="cCard uploadBox">
                    <div><img src="../img/upload.svg" /></div>
                    Laat mij feedback geven op het werk <br />van jouw studenten
                  </div>
                </div>
              </div>
            </div>
            <div class="eRow">
              <div class="col-md-5 mb-4 mb-md-0">
                <div class="reviewLeft">
                  <div class="eRow">
                    <div class="txt col-7">
                      Tamara Metz - software development docent
                      <div class="mt-4 txt">MboRijnIand</div>
                    </div>
                    <div class="text-center col-5">
                      <img src="../img/Image4.png" />
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-md-7 reviewRight">
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
              </div>
            </div>
          </div>
          <div class="greenBg">
            <div class="py-8 eContainer">
              <div class="eRow">
                <div class="col-sm-6"><img src="../img/Image5.png" /></div>
                <div class="col-sm-6">
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
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-window-item>
      <v-window-item value="Hbo">
        <div>
          <div class="eContainer">
            <div class="eRow">
              <div class="col-sm-7">
                <h4 class="text-h4 mb-3">
                  Ontmoet <span class="textGreen">onderwijsassistent</span> Omar
                </h4>
                <p class="mb-6" style="line-height: 1">
                  <small class="font-weight-bold text-subtitle-1"
                    >Hallo, mijn naam is Omar. 1k ben de assistent die je altijd al hebt gewild,<br />
                    maar nog nooit hebt kunnen hebben tot nu.</small
                  >
                </p>
                <v-btn class="btn rounded-0 cShadow">Leer meer over mij!</v-btn>
              </div>
              <div class="col-md-5 text-center text-md-end mt-4 mt-md-0">
                <img src="../img/Image2.png" alt="image" class="Image2" />
              </div>
            </div>
            <div class="eRow mt-4 mt-lg-0 gCard">
              <div class="col-md-4 my-3">
                <div class="cCard">
                  <img src="../img/star.svg" />
                  <h2>96%</h2>
                  <p>Mbo docenten besparen tijd met een Al assistent</p>
                </div>
              </div>
              <div class="col-md-4 my-3">
                <div class="cCard">
                  <img src="../img/star.svg" />
                  <h2>1.000+</h2>
                  <p>Mbo docenten gebruiken dagelijks een AI assistent</p>
                </div>
              </div>
              <div class="col-md-4 my-3">
                <div class="cCard">
                  <img src="../img/star.svg" />
                  <h2>50.000+</h2>
                  <p>Geeft een Eduface assistent feedback per maand</p>
                </div>
              </div>
            </div>
            <div class="mt-8 eRow">
              <div class="col-md-6 text-end">
                <img src="../img/Image3.png" class="Image3" />
              </div>
              <div class="col-md-6 mt-sm-4 mb-8 laatMij">
                <div class="mx-auto" style="max-width: 550px">
                  <h3 class="mt-sm-6 mt-md-14 mt-lg-16 text-h6 mb-6">
                    Laat mij jou ondersteunen bij jouw onderwijstaken! Dit is wat ik kan:
                  </h3>
                  <p>
                    <img src="../img/file.svg" class="me-1" /> Ik kan
                    <span class="textGreen">formatieve feedback</span> geven op de opdrachten van
                    jouw studenten
                  </p>
                  <p>
                    <img src="../img/box.svg" class="me-1" /> Ik kan onbeperkte veel
                    <span class="textGreen">oefenvragen</span> maken in jouw eigen digitale
                    leeromgeving.
                  </p>
                  <p>
                    <img src="../img/people.svg" class="me-1" /> Ik ben helemaal
                    <span class="textGreen">AVG</span> proof gebouwd en ik sla geen informatie op!
                  </p>
                  <div class="cCard uploadBox">
                    <div><img src="../img/upload.svg" /></div>
                    Laat mij feedback geven op het werk <br />van jouw studenten
                  </div>
                </div>
              </div>
            </div>
            <div class="eRow">
              <div class="col-md-5 mb-4 mb-md-0">
                <div class="reviewLeft">
                  <div class="eRow">
                    <div class="txt col-7">
                      Tamara Metz - software development docent
                      <div class="mt-4 txt">MboRijnIand</div>
                    </div>
                    <div class="text-center col-5">
                      <img src="../img/Image4.png" />
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-md-7 reviewRight">
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
              </div>
            </div>
          </div>
          <div class="greenBg">
            <div class="py-8 eContainer">
              <div class="eRow">
                <div class="col-sm-6"><img src="../img/Image5.png" /></div>
                <div class="col-sm-6">
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
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-window-item>
      <v-window-item value="Wo">
        <div>
          <div class="eContainer">
            <div class="eRow">
              <div class="col-sm-7">
                <h4 class="text-h4 mb-3">
                  Ontmoet <span class="textGreen">onderwijsassistent</span> Omar
                </h4>
                <p class="mb-6" style="line-height: 1">
                  <small class="font-weight-bold text-subtitle-1"
                    >Hallo, mijn naam is Omar. 1k ben de assistent die je altijd al hebt gewild,<br />
                    maar nog nooit hebt kunnen hebben tot nu.</small
                  >
                </p>
                <v-btn class="btn rounded-0 cShadow">Leer meer over mij!</v-btn>
              </div>
              <div class="col-md-5 text-center text-md-end mt-4 mt-md-0">
                <img src="../img/Image2.png" alt="image" class="Image2" />
              </div>
            </div>
            <div class="eRow mt-4 mt-lg-0 gCard">
              <div class="col-md-4 my-3">
                <div class="cCard">
                  <img src="../img/star.svg" />
                  <h2>96%</h2>
                  <p>Mbo docenten besparen tijd met een Al assistent</p>
                </div>
              </div>
              <div class="col-md-4 my-3">
                <div class="cCard">
                  <img src="../img/star.svg" />
                  <h2>1.000+</h2>
                  <p>Mbo docenten gebruiken dagelijks een AI assistent</p>
                </div>
              </div>
              <div class="col-md-4 my-3">
                <div class="cCard">
                  <img src="../img/star.svg" />
                  <h2>50.000+</h2>
                  <p>Geeft een Eduface assistent feedback per maand</p>
                </div>
              </div>
            </div>
            <div class="mt-8 eRow">
              <div class="col-md-6 text-end">
                <img src="../img/Image3.png" class="Image3" />
              </div>
              <div class="col-md-6 mt-sm-4 mb-8 laatMij">
                <div class="mx-auto" style="max-width: 550px">
                  <h3 class="mt-sm-6 mt-md-14 mt-lg-16 text-h6 mb-6">
                    Laat mij jou ondersteunen bij jouw onderwijstaken! Dit is wat ik kan:
                  </h3>
                  <p>
                    <img src="../img/file.svg" class="me-1" /> Ik kan
                    <span class="textGreen">formatieve feedback</span> geven op de opdrachten van
                    jouw studenten
                  </p>
                  <p>
                    <img src="../img/box.svg" class="me-1" /> Ik kan onbeperkte veel
                    <span class="textGreen">oefenvragen</span> maken in jouw eigen digitale
                    leeromgeving.
                  </p>
                  <p>
                    <img src="../img/people.svg" class="me-1" /> Ik ben helemaal
                    <span class="textGreen">AVG</span> proof gebouwd en ik sla geen informatie op!
                  </p>
                  <div class="cCard uploadBox">
                    <div><img src="../img/upload.svg" /></div>
                    Laat mij feedback geven op het werk <br />van jouw studenten
                  </div>
                </div>
              </div>
            </div>
            <div class="eRow">
              <div class="col-md-5 mb-4 mb-md-0">
                <div class="reviewLeft">
                  <div class="eRow">
                    <div class="txt col-7">
                      Tamara Metz - software development docent
                      <div class="mt-4 txt">MboRijnIand</div>
                    </div>
                    <div class="text-center col-5">
                      <img src="../img/Image4.png" />
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-md-7 reviewRight">
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
              </div>
            </div>
          </div>
          <div class="greenBg">
            <div class="py-8 eContainer">
              <div class="eRow">
                <div class="col-sm-6"><img src="../img/Image5.png" /></div>
                <div class="col-sm-6">
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
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-window-item>
    </v-window>

    <div class="eContainer py-6">
      <h3>FAQs</h3>
      <v-expansion-panels variant="inset" class="mt-4">
        <v-expansion-panel
          title="How do I create a new assignment?"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"
        >
        </v-expansion-panel>
      </v-expansion-panels>
      <v-expansion-panels variant="inset" class="mt-4">
        <v-expansion-panel
          title="How can I track student progress?"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"
        >
        </v-expansion-panel>
      </v-expansion-panels>
      <v-expansion-panels variant="inset" class="mt-4">
        <v-expansion-panel
          title="Having trouble logging in?"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"
        >
        </v-expansion-panel>
      </v-expansion-panels>
    </div>
  </div>
</template>

<style>
.v-slide-group__container {
  display: block !important;
  width: 100%;
  text-align: center;
}
.v-slide-group__content {
  display: inline-block !important;
  margin: auto !important;
  background-color: #f2f2f2;
  border-radius: 45px;
  padding: 5px;
}
.v-slide-group__content button {
  border-radius: 45px !important;
  height: 38px !important;
}
.v-tab__slider {
  display: none;
}
.v-slide-group__content .v-btn {
  background-color: #f2f2f2 !important;
  color: #000 !important;
}
.v-btn.v-slide-group-item--active {
  background-color: #fff !important;
}
button.v-expansion-panel-title {
  background-color: #fff !important;
  color: #000 !important;
  padding: 0 0 0 15px !important;
  margin: 0 !important;
  display: block;
  width: calc(100% - 15px);
  min-height: 38px !important;
  font-weight: bold;
  font-size: 18px !important;
  line-height: 2;
}
v-expansion-panels {
  padding: 0 !important;
}
.v-expansion-panel {
  border-radius: 15px !important;
}

.v-expansion-panels--variant-inset > .v-expansion-panel--active {
  max-width: 100% !important;
}
</style>

<style scoped>
@import '../assets/grid.css';
*,
span {
  font-family: 'League Spartan', sans-serif !important;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
  color: #414042;
}
@media (max-width: 576px) {
  .edHome {
    margin: 0 15px;
  }
}

button {
  margin-top: 0 !important;
}
.mainHeading {
  letter-spacing: 2px;
}
.btn {
  background-color: #00e075 !important;
  box-shadow: none;
  font-weight: 600;
  text-transform: capitalize;
  font-size: 16px;
  padding: 15px 25px;
  height: auto !important;
  color: #000 !important;
}
.loginBtn {
  background: transparent !important;
  color: #000 !important;
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
.textGreen {
  color: #2c8a62;
}

.topCard {
  background-color: #ebebeb;
  border: 1px solid #686868;
  box-shadow: rgb(48 63 79) 50px 50px 56px -9px !important;
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
  cursor: pointer;
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
.gCard img {
  width: 40px;
  margin-bottom: 20px;
}
.gCard h2 {
  margin-bottom: 20px;
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
