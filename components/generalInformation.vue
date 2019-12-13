<template>
  <!-- General Information -->
  <div class="general_info d-flex flex-xl-column flex-md-row flex-column">
    <div>
      <div class="general_info_image">
        <b-img
          class="background_image"
          src="images/researcherImage.jpg"
          fluid
          alt="Responsive image"
        ></b-img>
      </div>
    </div>
    <div class="general_info_content">
      <div
        class="general_info_content_inner mCustomScrollbar"
        data-mcs-theme="minimal-dark"
      >
        <div class="general_info_title">General Information</div>
        <ul class="general_info_list">
          <li class="d-flex flex-row align-items-center justify-content-start">
            <div
              class="general_info_icon d-flex flex-column align-items-start justify-content-center"
            >
              <img src="images/icon_1.png" alt />
            </div>
            <div class="general_info_text">
              Name:
              <span>{{ researcher.fullname }}</span>
            </div>
          </li>
          <li class="d-flex flex-row align-items-center justify-content-start">
            <div
              class="general_info_icon d-flex flex-column align-items-start justify-content-center"
            ></div>
            <div class="general_info_text">
              Location:
              <span>London UK</span>
            </div>
          </li>
          <li class="d-flex flex-row align-items-center justify-content-start">
            <div
              class="general_info_icon d-flex flex-column align-items-start justify-content-center"
            >
              <img src="images/icon_2.png" alt />
            </div>
            <div class="general_info_text">
              Date of Birth:
              <span>August 25, 1991</span>
            </div>
          </li>
          <li class="d-flex flex-row align-items-center justify-content-start">
            <div
              class="general_info_icon d-flex flex-column align-items-start justify-content-center"
            >
              <img src="images/icon_3.png" alt />
            </div>
            <div class="general_info_text">
              <a href="mailto:contact@linque.com?subject=Job_Inquiry"
                >contactme@templatename.com</a
              >
            </div>
          </li>
          <li class="d-flex flex-row align-items-center justify-content-start">
            <div
              class="general_info_icon d-flex flex-column align-items-start justify-content-center"
            >
              <img src="images/icon_4.png" alt />
            </div>
            <div class="general_info_text">+76 6524 567862 763</div>
          </li>
          <li class="d-flex flex-row align-items-center justify-content-start">
            <div
              class="general_info_icon d-flex flex-column align-items-start justify-content-center"
            >
              <img src="images/icon_5.png" alt />
            </div>
            <div class="general_info_text">
              <a href="mailto:contact@linque.com">www.mytemplatename.com</a>
            </div>
          </li>
        </ul>

        <!-- Social -->
        <div class="social_container">
          <ul class="d-flex flex-row align-items-start justify-content-start">
            <li>
              <a href="#">
                <i class="fa fa-google-plus" aria-hidden="true"></i>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fa fa-pinterest" aria-hidden="true"></i>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fa fa-facebook" aria-hidden="true"></i>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fa fa-twitter" aria-hidden="true"></i>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
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
