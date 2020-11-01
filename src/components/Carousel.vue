<template>
  <v-row no-gutters>
    <v-carousel cycle hide-delimiters>
      <v-carousel-item src="@/assets/img/bg-familia-wide.png">
        <v-row class="fill-height" align="center" justify="center">
          <div
            class="carousel-text d-flex flex-column align-center text-center"
          >
            <h2>Distribuindo qualidade de vida</h2>
            <p>Atendemos toda a Baixada Santista</p>
            <v-btn outlined max-width="130px" rounded="xl" class="carousel-btn">
              SAIBA MAIS <v-icon>mdi-arrow-right</v-icon>
            </v-btn>
          </div>
        </v-row>
      </v-carousel-item>
      <v-carousel-item src="@/assets/img/bg-nutren.jpg">
        <v-row class="fill-height" align="center" justify="center">
          <div
            class="carousel-text d-flex flex-column align-center text-center"
          >
            <h2>Distribuindo qualidade de vida</h2>
            <p>Atendemos toda a Baixada Santista</p>
            <v-btn outlined max-width="130px" rounded="xl" class="carousel-btn">
              SAIBA MAIS <v-icon>mdi-arrow-right</v-icon>
            </v-btn>
          </div>
        </v-row>
      </v-carousel-item>
    </v-carousel>
    <v-row no-gutters align="center" justify="center">
      <v-card v-if="!isMobile()" class="d-flex card-services" width="70%">
        <v-col
          class="d-flex flex-column align-start justify-start"
          cols="12"
          sm="1"
          md="3"
        >
          <v-icon size="40px" color="black">mdi-needle</v-icon>
          <h5 class="card-title">Agilidade</h5>
          <p class="card-text">
            entrega rápida e prática em toda a Baixada Santista.
          </p>
        </v-col>
        <v-col
          class="d-flex flex-column align-start justify-start"
          cols="12"
          sm="1"
          md="3"
        >
          <v-icon size="40px" color="black">mdi-run</v-icon>
          <h5 class="card-title">Produtos Nestlé</h5>
          <p class="card-text">Diversos produtos Nestlé Health Science.</p>
        </v-col>
        <v-col
          class="d-flex flex-column align-start justify-start"
          cols="12"
          sm="1"
          md="3"
        >
          <v-icon size="40px" color="black">mdi-heart-pulse</v-icon>
          <h5 class="card-title">Nutrição</h5>
          <p class="card-text">Alimentos que garantem uma nutrição completa.</p>
        </v-col>
        <v-col
          class="d-flex flex-column align-start justify-start"
          cols="12"
          sm="1"
          md="3"
        >
          <v-icon size="40px" color="black">mdi-atom</v-icon>
          <h5 class="card-title">Especialização</h5>
          <p class="card-text">
            Atendimento por equipe especializada de nutricionista e farmacêutica
          </p>
        </v-col>
      </v-card>
    </v-row>
  </v-row>
</template>

<script>
export default {
  methods: {
    isMobile() {
      if (
        /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(
          navigator.userAgent
        )
      ) {
        return true;
      } else {
        return false;
      }
    },
  },
};
</script>

<style lang="scss">
.row {
  .v-carousel {
    .v-carousel__item {
      .carousel-text {
        .carousel-btn:hover {
          color: black;
          background-color:rgba(241, 241, 241, 0.445);
        }
      }
    }
  }
  .row {
    .card-services {
      top: -97px;
      .v-icon {
        border-bottom: 2px solid #000;
        margin-bottom: 13px;
      }
      .card-title {
        font-size: 17px;
        margin-bottom: 15px;
      }
      .card-text {
        font-size: 14px;
      }
      .col-12:nth-child(1) {
        background-color: rgb(255, 136, 28);
      }
      .col-12:nth-child(2) {
        background-color: rgb(255, 145, 46);
      }
      .col-12:nth-child(3) {
        background-color: rgb(255, 159, 72);
      }
      .col-12:nth-child(4) {
        background-color: rgb(255, 172, 96);
      }
    }
  }
}
</style>
