<template>
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
</template>

<script>
export default {

}
</script>

<style lang="scss">
.contact {
    margin-top: 80px;
    margin-bottom: 50px;
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
</style>