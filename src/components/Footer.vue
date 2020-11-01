<template>
  <footer class="footer">
    <v-row class="flex-column" no-gutters>
      <v-col class="pa-10" cols="12" md="3">
        <div class="div-img">
          <v-img src="@/assets/img/logo.png"></v-img>
        </div>
      </v-col>
      <v-col class="pa-8" cols="12" md="12">
        <v-row no-gutters>
          <v-col cols="12" md="4">
            <v-icon size="60px" class="mb-10" color="rgb(255, 136, 28)">
              mdi-map-marker
            </v-icon>
            <p>Rua Antônio Bento, 79 – loja 2</p>
            <p>Vila Mathias I Santos – SP I CEP: 11075-260</p>
          </v-col>
          <v-col cols="12" md="4">
            <v-icon size="60px" class="mb-10" color="rgb(255, 136, 28)">
              mdi-email-newsletter
            </v-icon>
            <p>
              <a href="mailto:vendas@haverim.com.br">
                vendas@haverim.com.br
              </a>
            </p>
          </v-col>
          <v-col class="d-flex flex-column align-end" cols="12" md="4">
            <v-icon size="60px" class="mb-10" color="rgb(255, 136, 28)">
              mdi-phone-in-talk
            </v-icon>
            <p>
              <a href="tel:+551333217933">
                13 3321.7933
              </a>
            </p>
            <p>
              <a href="tel:+5513974213810">
                13 97421.3810
              </a>
            </p>
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="12" md="12">
        <h1>3</h1>
      </v-col>
    </v-row>
  </footer>
</template>

<script>
export default {};
</script>

<style lang="scss">
footer {
  margin-top: 50px;
  .row {
    .div-img {
      border-top: 2px solid rgb(255, 136, 28);
      .v-image {
        max-width: 70%;
        margin: 20px;
      }
    }
    .col-12:nth-child(2) {
      background-color: #f0f0f0;
      p {
        line-height: 10px;
      }
      a {
        text-decoration: none;
        color: black;
      }
      a:hover {
        text-decoration: none;
        color: black;
        font-weight: 750;
      }
    }
  }
}
</style>
