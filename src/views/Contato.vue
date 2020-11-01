import Contact from '@/components/FaleConosco.vue';
<template>
  <div class="contact">
    <v-row class="top-content" no-gutters>
      <v-img max-height="" src="@/assets/img/banner.png">
        <v-row align="center" justify="center" class="flex-column" no-gutters>
          <h1>Contato</h1>

          <h3>Faça cotações, tire dúvidas ou venha nos visitar!</h3>
        </v-row>
      </v-img>
    </v-row>

    <v-row
      align="center"
      class="midle-content text-center flex-column mt-14"
      no-gutters
    >
      <v-row class="title mb-15" no-gutters>
        <h1>Fale Conosco</h1>
      </v-row>

      <v-row class="text-content flex-column">
        <p>
          Entre em contato conosco através do e-mail: vendas@haverim.com.br, ou,
          preenchendo o formulário dessa página.
        </p>
        <p>
          Solicite uma visita de nossa equipe, teremos muito prazer em
          atendê-lo.
        </p>
        <p>
          Envie, também, suas dúvidas e sugestões, sua opinião é muito
          importante para nós.
        </p>
        <p>Se preferir, entre em contato pelos telefones:</p>
      </v-row>

      <v-row class="tel">
        <a class="mr-2" href="tel:+551333217933">13 3321.7933</a>
        <a class="ml-2" href="tel:+5513974213810">13 97421.3810</a>
      </v-row>
    </v-row>


    <Contact />
  </div>
</template>

<script>
import Contact from "@/components/FaleConosco.vue"

export default {
  components: {
    Contact
  }
};
</script>

<style lang="scss">
.contact {
  .row {
    .v-image {
      height: 200px;
      .v-responsive__content {
        display: flex;
        h1 {
          color: white;
          font-size: 45px;
        }
        h3 {
          color: white;
          font-weight: 400;
          font-size: 27px;
        }
      }
    }
  }
  .midle-content {
    .title {
      border-bottom: 2px solid rgb(255, 136, 28);
      h1 {
        font-size: 32px;
        color: rgb(165, 165, 165);
      }
    }
    .tel {
      a {
        text-decoration: none;
        color: rgb(165, 165, 165);
      }
      :hover {
        text-decoration: none;
        font-weight: 750;
      }
    }
  }
}
</style>
