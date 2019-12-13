<template>
  <b-container fluid>
    <div class="content_container">
      <div
        class="main_content_outer d-flex flex-xl-row flex-column align-items-start justify-content-start"
      >
        <general-information></general-information>
        <!-- Main Content -->

        <div class="main_content">
          <div
            class="main_title_container d-flex flex-column align-items-start justify-content-end"
          >
            <div class="main_subtitle">{{ researcher.alias }}</div>
            <div class="main_title">{{ researcher.fullname }}</div>
          </div>
          <div
            class="main_content_scroll mCustomScrollbar"
            data-mcs-theme="minimal-dark"
          >
            <div class="about_content">
              <div class="about_title">Descripción</div>
              <div class="about_text">
                <p>{{ researcher.description }}</p>
              </div>

              <!-- Loaders -->

              <div class="loaders clearfix">
                <!-- Loader -->
                <skill-loader :percent="45"></skill-loader>
                <div class="loader_container">
                  <div class="loader" data-perc="0.75"></div>
                  <div class="loader_content text-center">
                    <div class="loader_title">intuition</div>
                    <div class="loader_subtitle">
                      Etiam nec odio vestibulum est.
                    </div>
                  </div>
                </div>

                <!-- Loader -->
                <div class="loader_container">
                  <div class="loader" data-perc="0.25"></div>
                  <div class="loader_content text-center">
                    <div class="loader_title">pure luck</div>
                    <div class="loader_subtitle">
                      Vestibulum est mattis effic.
                    </div>
                  </div>
                </div>

                <!-- Loader -->
                <div class="loader_container">
                  <div class="loader" data-perc="0.95"></div>
                  <div class="loader_content text-center">
                    <div class="loader_title">awesomeness</div>
                    <div class="loader_subtitle">
                      Vestibulum est mattis effic.
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </b-container>
</template>

<script>
import skillLoader from "@/components/skillLoader";
import generalInformation from "@/components/generalInformation";

export default {
  head: {
    link: [
      { rel: "stylesheet", href: require("@/assets/styles/contact.css") },
      {
        rel: "stylesheet",
        href: require("@/assets/styles/main_styles.css")
      }
    ]
  },
  components: {
    generalInformation,
    skillLoader
  },
  data() {
    return {
      researcher: {
        fullname: "Juan Ubaldo Jimenez Castilla",
        alias: "Investigador",
        location: "Tacna",
        birthday: "16-05-62",
        email: "jjimenezc16@gmail.com",
        phone: "+51982426891",
        ctiVitae:
          "http://dina.concytec.gob.pe/appDirectorioCTI/VerDatosInvestigador.do?id_investigador=57992",
        description:
          "Docente Principal a tiempo completo en la Escuela Profesional de Ingeniería de Sistemas e Informática, Facultad de Ingeniería y Arquitectura, Universidad José Carlos Mariátegui, Moquegua, Perú. Ingeniero de Sistemas con Grado de Doctor en sistemas, Doctor en Gestion y Ciencias de la Educación. PhD Systems Information, Atlantic International University, EEUU. Ex Docente Asociado y Director de Escuela Ingeniería Informática y Sistemas, Facultad de Ingeniería, Universidad Nacional Jorge Basadre Grohmann, Tacna, Perú. Ex Decano de Facultad de Ingeniería, Universidad José Carlos Mariátegui, Moquegua, Perú. Evaluador Externo CONEAU-SINEACE. Área de Investigación: Sistemas Rizomáticos y Sistemas Cognitivos."
      }
    };
  }
};
</script>

<style lang="scss" scoped></style>
