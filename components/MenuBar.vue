<template>

  <v-row class="topBar">
    <v-col cols="12" xl="6" lg="6" md="6" class="d-flex justify-center mt-2 justify-xl-start justify-lg-start justify-md-start">
      <v-img
        :src="require('../assets/images/logo.png')"
        height="50px"
        contain
      ></v-img>
    </v-col>
    <v-col class="d-flex justify-center flex-wrap justify-xl-end justify-lg-end justify-md-end" cols="12" xl="6" lg="6" md="6">
      <v-btn depressed large href="#about" class="mr-2">About</v-btn>
      <v-btn depressed large href="#portfolio" class="mr-2">Portfolio</v-btn>
      <v-btn depressed large href="#services" class="mr-2">Services</v-btn>
    </v-col>
  </v-row>

</template>
<style>
.topBar {
    background-color: #272727;
}
</style>