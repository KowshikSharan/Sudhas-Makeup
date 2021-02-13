 <template>
  <v-footer app fixed color="#FEDBD0">
    <v-row class="d-flex">
      <v-col
        cols="12"
        xl="4"
        lg="4"
        md="4"
        class="d-flex align-center justify-center"
      >
        <v-row class="d-flex justify-center">
          <v-btn
            text
            href="https://www.instagram.com/sudha_instaura_artifex/?hl=en"
            target="blank"
            color="#442C2E"
          >
            <v-icon x-large color="#442C2E">mdi-instagram</v-icon>
            <p class="text">@sudha_instaura_artifex</p>
          </v-btn>
        </v-row>
      </v-col>
      <v-col cols="12" xl="4" lg="4" md="4" class="d-flex justify-center">
        <v-icon x-large color="#442C2E">mdi-email</v-icon>
        <p class="text">sudharavishankar97851@gmail.com</p>
      </v-col>
      <v-col cols="12" xl="4" lg="4" md="4" class="d-flex justify-center">
        <v-icon large color="#442C2E">mdi-cellphone</v-icon>
        <p class="text">+91 766 705 0279</p>
      </v-col>
    </v-row>
  </v-footer>
</template>
<style lang="scss">
@import '~/assets/variables.scss';
.text {
  color: $text-color;
}
</style>