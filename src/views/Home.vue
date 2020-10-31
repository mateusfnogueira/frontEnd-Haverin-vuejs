<template>
  <div class="home">
    <Carousel />

    <v-row
      align="center"
      justify="center"
      class="about text-center mb-15"
      no-gutters
    >
      <v-col class="d-flex justify-center" cols="12" sm="12" md="12">
        <h1>A Haverin</h1>
      </v-col>
      <v-col cols="12" md="5">
        <v-img src="@/assets/img/equipeHaverim.png"></v-img>
      </v-col>
      <v-col cols="12" md="6" class="pa-10">
        <p>
          A Haverim atua desde 2012 oferecendo a seus clientes o que há de
          melhor em nutrição clínica e dieta enteral.
        </p>
        <p>
          Comercializamos produtos testados e aprovados por uma equipe de
          nutricionistas das mais renomadas marcas como Nestlé, Humalin e Naiak.
        </p>
        <p>
          Além da linha de alimentação enteral e suplementação para pacientes
          que precisam de cuidados especiais oferecemos também opções para quem
          busca longevidade, prevenção, manutenção da saúde e bem estar.
        </p>
        <p>
          Nosso principal diferencial é a atenção aos nossos clientes de forma
          individualizada e personalizada. Sabemos que cada um que nos procura é
          o amor da vida de alguém e aqui, na Haverim, trabalhamos com respeito
          e dedicação, porque toda história de amor merece os momentos mais
          felizes possíveis.
        </p>
      </v-col>
    </v-row>

    <v-row
      class="highlights text-center"
      align="center"
      justify="center"
      no-gutters
    >
      <v-col class="d-flex flex-column align-center" cols="12" sm="12" md="12">
        <h3>
          Confira
        </h3>
        <h1>
          Nossos Destaques
        </h1>
      </v-col>
      <v-col cols="12" sm="12" md="12">
        <v-img class="mt-16" src="@/assets/img/destaques1.png"></v-img>
      </v-col>
    </v-row>

    <v-row
      class="products text-center"
      align="center"
      justify="center"
      no-gutters
    >
      <v-col cols="12" sm="12" md="6" lg="3">
        <v-img src="@/assets/img/trophic.png"></v-img>
      </v-col>
      <v-col cols="12" sm="12" md="6" lg="3">
        <v-img src="@/assets/img/trophic.png"></v-img>
      </v-col>
      <v-col cols="12" sm="12" md="6" lg="3">
        <v-img src="@/assets/img/trophic.png"></v-img>
      </v-col>
      <v-col cols="12" sm="12" md="6" lg="3">
        <v-img src="@/assets/img/trophic.png"></v-img>
      </v-col>
    </v-row>
  </div>
</template>

<script>
// @ is an alias to /src
import Carousel from "@/components/Carousel.vue";

export default {
  name: "Home",
  data() {
    return {};
  },
  components: {
    Carousel,
  },
};
</script>

<style lang="scss">
.home {
  .about {
    h1 {
      color: rgb(165, 165, 165);
      font-size: 40px;
      font-weight: 750;
      border-bottom: 2px solid rgb(255, 136, 28);
      max-width: 200px;
    }
    p {
      color: rgb(165, 165, 165);
      font-size: 17px;
      margin-bottom: 0px;
    }
  }
  .highlights {
    h1 {
      color: rgb(165, 165, 165);
      font-size: 40px;
      font-weight: 750;
      border-bottom: 2px solid rgb(255, 136, 28);
      max-width: 500px;
    }
    h3 {
      color: rgb(165, 165, 165);
      font-size: 18px;
      max-width: 200px;
    }
  }
}
</style>
