<template>
  <footer class="footer">
    <v-row class="flex-column" no-gutters>
      <v-col class="pa-10" cols="12" md="3">
        <div class="div-img">
          <v-img src="@/assets/img/logo.png"></v-img>
        </div>
      </v-col>
      <v-col class="pa-8 col-branca" cols="12" md="12">
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
        <v-row align="center" no-gutters>
          <v-col class="mt-2 d-flex justify-center" cols="12" md="4">
            <p>2018 - Haverim - Todos os direitos reservados.</p>
          </v-col>
          <v-col class="d-flex justify-center" cols="12" md="4">
            <v-img max-width="30%" src="@/assets/img/logo-marca-site.png"></v-img>
          </v-col>
          <v-col class="d-flex flex-column col-menu" cols="12" md="4">
            <v-list class="d-flex menu-footer">
              <v-list-item @click="() => {}">
                <router-link to="/">Home</router-link>
              </v-list-item>
              <v-list-item @click="() => {}">
                <router-link to="/about">O Grupo</router-link>
              </v-list-item>
              <v-list-item @click="() => {}">
                <router-link to="/atuacao">Atuação</router-link>
              </v-list-item>
              <v-list-item @click="() => {}">
                <router-link to="/produtos">Produtos</router-link>
              </v-list-item>
              <v-list-item @click="() => {}">
                <router-link to="/contato">Contato</router-link>
              </v-list-item>
            </v-list>
          </v-col>
        </v-row>
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
    .col-branca {
      background-color: #f0f0f0;
    }
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
    .menu-footer {
        a {
            font-size: 10px;
        }
        .col-menu {
            align-items: initial;
        }
    }
  }
}
</style>
