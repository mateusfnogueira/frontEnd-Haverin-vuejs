<template>
  <header class="header">
    <v-app-bar flat color="white">
      <v-menu v-if="isMobile()" left bottom>
        <template v-slot:activator="{ on, attrs }">
          <v-btn icon v-bind="attrs" v-on="on">
            <v-app-bar-nav-icon></v-app-bar-nav-icon>
          </v-btn>
        </template>

        <v-list class="menu-header-mobile">
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
      </v-menu>

      <v-col class="col-img" cols="12" sm="2" md="3">
        <v-img
          src="@/assets/img/logo.png"
          contain
          max-width="130px"
          aspect-ratio="1"
        ></v-img>
      </v-col>

      <v-col
        v-if="!isMobile()"
        class="d-flex flex-column"
        cols="12"
        sm="0"
        md="5"
      >
        <v-list class="d-flex menu-header">
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

      <v-col cols="12" sm="4" md="3">
        <v-card
          rounded="xl"
          max-width="170px"
          max-height="45px"
          class="text-center d-flex align-center card-wpp"
          color="green"
        >
          <v-card-text>
            <a href="https://api.whatsapp.com/send?l=pt&phone=5513972449999">
              <v-icon>mdi-whatsapp</v-icon>
            13 97244.9999
            </a>
          </v-card-text>
        </v-card>
      </v-col>
    </v-app-bar>
  </header>
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
.header {
  .v-app-bar {
    .v-toolbar__content {
      justify-content: space-between;
      .col-img {
        max-width: 160px;
        .v-image {
        }
      }
      .v-card {
        .v-card__text {
          font-weight: 800;
        }
      }
    }
    .card-wpp {
      a {
        text-decoration: none;
        color: black;
      }
      a:hover {
        text-decoration: none;
        color: black;
      }
    }
  }
  .menu-header {
    a {
      text-decoration: none;
      color: black ;
    }:hover {
      text-decoration: none;
      color: rgb(255, 136, 28) ;
      font-weight: 750;
    }
  }
}
</style>
