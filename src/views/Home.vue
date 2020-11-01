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
        <a class="d-flex flex-column align-center" href="#">
          <v-img width="60%" src="@/assets/img/trophic.png"></v-img>
          <p>Trophic 1.5 - Hipercalórica 1.5 kcal por ml</p>

          <p>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
          </p>

          <p>R$50,00</p>
        </a>
      </v-col>
      <v-col cols="12" sm="12" md="6" lg="3">
        <a class="d-flex flex-column align-center" href="#">
          <v-img width="38%" src="@/assets/img/resource.png"></v-img>
          <p>Trophic 1.5 - Hipercalórica 1.5 kcal por ml</p>

          <p>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
          </p>

          <p>R$50,00</p>
        </a>
      </v-col>
      <v-col cols="12" sm="12" md="6" lg="3">
        <a class="d-flex flex-column align-center" href="#">
          <v-img width="60%" src="@/assets/img/nutrenJunior.png"></v-img>
          <p>Trophic 1.5 - Hipercalórica 1.5 kcal por ml</p>

          <p>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
          </p>

          <p>R$50,00</p>
        </a>
      </v-col>
      <v-col cols="12" sm="12" md="6" lg="3">
        <a class="d-flex flex-column align-center" href="#">
          <v-img width="60%" src="@/assets/img/trophicSoya.png"></v-img>
          <p>Trophic 1.5 - Hipercalórica 1.5 kcal por ml</p>

          <p>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
            <v-icon size="25px">mdi-star</v-icon>
          </p>

          <p>R$50,00</p>
        </a>
      </v-col>
    </v-row>

    <v-row class="contact text-center">
      <v-col cols="12" sm="12" md="6" lg="6">
        <v-img height="90%" src="@/assets/img/contato-img.png"></v-img>
      </v-col>
      <v-col cols="12" sm="12" md="6" lg="6">
        <v-row class="flex-column" align="center" justify="center" no-gutters>
          <h2>Solicite uma visita</h2>
          <p style="line-height: 3px;">
            Estamos sempre prontos para atender com
          </p>
          <p style="line-height: 3px;">maior agilidade e qualidade possível.</p>

          <p>Telefones: (13) 3321.7933 e (13) 97421.3810</p>

          <v-form>
            <v-text-field label="Nome" outlined rounded required></v-text-field>
            <v-text-field
              label="E-mail"
              outlined
              rounded
              required
            ></v-text-field>
            <v-text-field
              label="Telefone"
              outlined
              rounded
              required
            ></v-text-field>
            <v-text-field
              label="Assunto"
              outlined
              rounded
              required
            ></v-text-field>
            <v-textarea outlined rounded rows="5"> </v-textarea>
            <v-btn outlined>Limpar</v-btn>
            <v-btn outlined>Enviar</v-btn>
          </v-form>
        </v-row>
      </v-col>
    </v-row>

    <v-row class="blog text-center">
      <v-col cols="12" sm="12" md="12" class="d-flex justify-center blog-title">
        <h1>Dicas de Saúde</h1>
      </v-col>
      <v-row
        align="center"
        class="justify-space-around text-center blog-info"
        no-gutters
      >
        <v-col cols="12" sm="7" md="4" class="d-flex flex-column align-center">
          <img width="80%" src="@/assets/img/blog-img.png" alt="" />

          <h2>Saúde Cognitiva</h2>

          <p>
            Declínios na saúde cognitiva associados à idade podem ser normais,
            mas eles não precisam ser um problema grave. Tomar as medidas
            necessárias para manter e até melhorar a saúde cognitiva durante o
            processo de envelhecimento é importante. Saber mais sobre o que
            influencia o cérebro e cognição são aspectos que podem ajudar.
          </p>
        </v-col>
        <v-col cols="12" sm="7" md="4" class="d-flex flex-column align-center">
          <img width="80%" src="@/assets/img/blog-img.png" alt="" />

          <h2>Saúde Cognitiva</h2>

          <p>
            Declínios na saúde cognitiva associados à idade podem ser normais,
            mas eles não precisam ser um problema grave. Tomar as medidas
            necessárias para manter e até melhorar a saúde cognitiva durante o
            processo de envelhecimento é importante. Saber mais sobre o que
            influencia o cérebro e cognição são aspectos que podem ajudar.
          </p>
        </v-col>
      </v-row>
    </v-row>

    <v-row class="map text-center">
      <v-img src="@/assets/img/map.png">
        <v-row class="flex-column " align="center" justify="center" no-gutters>
          <h2>
            Atuamos em toda a Baixada Santista,<br />
            Vale do Ribeira e Litoral Norte.
          </h2>
          <p>200 km dentro do Estado de São Paulo</p>
          <v-btn outlined rounded="xl" color="white">
            SAIBA MAIS
          </v-btn>
        </v-row>
      </v-img>
    </v-row>
  </div>
</template>

<script>
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

<style lang="scss" scoped>
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
    margin-top: 120px;
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
  .products {
    margin-top: 130px;
    a {
      text-decoration: none;
      color: rgb(165, 165, 165);
      i {
        color: goldenrod;
      }
    }
    :hover {
      text-decoration: none;
      font-weight: 750;
    }
  }
  .contact {
    margin-top: 140px;
    h2 {
      font-size: 22px;
      color: rgb(165, 165, 165);
    }
    p {
      font-size: 14px;
      color: rgb(165, 165, 165);
    }
    form {
      width: 80%;
      fieldset {
        height: 90%;
      }
    }
  }

  .blog {
    .blog-title {
      margin-bottom: 30px;
      h1 {
        border-bottom: 2px solid rgb(255, 136, 28);
        font-size: 32px;
        color: rgb(165, 165, 165);
      }
    }
    .blog-info {
      img::before {
        width: 30%;
        height: 50%;
        background-color: rgb(255, 136, 28);
      }
      h2 {
        font-size: 26px;
        color: rgb(165, 165, 165);
      }
      p {
        font-size: 16px;
        color: rgb(165, 165, 165);
      }
    }
  }
  .map {
    margin-top: 130px;
    .v-image {
      display: flex;
      align-items: center;
      .v-responsive__content {
        h2 {
          color: white;
        }
        p {
          color: white;
        }
        .v-btn:hover {
          color: black !important;
          background-color: rgba(241, 241, 241, 0.445);
        }
      }
    }
  }
}
</style>
