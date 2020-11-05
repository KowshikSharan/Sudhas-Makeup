<template>

  <v-row class="topBar">
    <v-col cols="12" xl="3" lg="3" md="3" class="d-flex justify-center mt-2 justify-xl-start justify-lg-start justify-md-start">
      <v-img
        :src="require('../assets/images/logo.png')"
        height="50px"
        contain
       />
    </v-col>
    <v-col class="d-flex justify-center flex-wrap justify-xl-end justify-lg-end justify-md-end" cols="12" xl="9" lg="9" md="9">
      <v-btn text color="#442C2E" depressed large href="#about" class="mr-2 buttonText">About</v-btn>
      <v-btn text color="#442C2E" depressed large href="#portfolio" class="mr-2">Portfolio</v-btn>
      <v-btn text color="#442C2E" depressed large href="#services" class="mr-2">Services</v-btn>
    </v-col>
  </v-row>

</template>
<style scoped lang="scss">
@import '@/assets/variables.scss';

.topBar {
    background-color: $primary-color;
}
.buttonText {
  background-color: $primary-color;
  color: $text-color;
}
.test {
  background-color: yellow;;
}
</style>