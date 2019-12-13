<template>
  <b-container fluid
    ><div class="content_container">
      <div
        class="main_content_outer d-flex flex-xl-row flex-column align-items-start justify-content-start"
      >
        <!-- General Information -->
        <general-information></general-information>

        <!-- Main Content -->

        <div class="main_content">
          <div
            class="main_title_container d-flex flex-column align-items-start justify-content-end"
          >
            <!-- <div class="main_subtitle">What I am good at</div> -->
            <div class="main_title">Mi Educación</div>
          </div>
          <div
            class="main_content_scroll mCustomScrollbar"
            data-mcs-theme="minimal-dark"
          >
            <!-- Education -->

            <div
              class="education"
              v-for="(item, itemId) in education"
              :key="itemId"
            >
              <!-- Education Item -->
              <div
                class="edu_item d-flex flex-lg-row flex-column align-items-start justfy-content-start"
              >
                <div>
                  <div class="edu_year">{{ item.year }}</div>
                </div>
                <div>
                  <div class="edu_image">
                    <img :src="item.universityImg" alt="" />
                  </div>
                </div>
                <div class="edu_content">
                  <div class="edu_title_container">
                    <div class="edu_title">{{ item.university }}</div>
                    <div class="edu_subtitle">
                      {{ item.degree }} - {{ item.title }} - {{ item.country }}
                    </div>
                  </div>
                  <div class="edu_text">
                    <p>
                      {{ item.description }}
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div></b-container
  >
</template>

<script>
import generalInformation from "@/components/generalInformation";
export default {
  components: {
    generalInformation
  },
  head: {
    link: [
      { rel: "stylesheet", href: require("@/assets/styles/education.css") }
    ]
  },
  data() {
    return {
      education: [
        {
          year: 2012,
          university: "UNIVERSIDAD JOSÉ CARLOS MARIÁTEGUI",
          country: "Perú",
          degree: "LICENCIADO / TÍTULO",
          title: "SEGUNDA ESPECIALIDAD",
          description: "Curse mi especialidad en tal",
          universityImg:
            "https://carrerasuniversitarias.pe/logos/original/logo-universidad-jose-carlos-mariategui.png"
        },
        {
          year: 2013,
          university: "UNIVERSIDAD PRIVADA DE TACNA",
          country: "Perú",
          degree: "LICENCIADO / TÍTULO",
          title: "INGENIERO DE SISTEMAS",
          description: "Curse mi especialidad en tal",
          universityImg:
            "https://1.bp.blogspot.com/-fiCqijmx7UY/Won9KRnJa0I/AAAAAAAAAII/b6s8IbQxqosNaboSBHLpNH_189pil13ZACLcBGAs/s1600/upt-resultados.jpg"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped></style>
