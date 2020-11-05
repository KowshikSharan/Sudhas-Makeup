<template>
  <v-row class="ma-7 d-flex justify-center">
    <h1 class="aboutText" id="about">About</h1>
    <v-row class="about">
      <v-col cols="12" xl="3" lg="3" md="3" class="d-flex justify-center">
          <v-img :src="require('../assets/images/about.png')" max-width="200px" contain></v-img>
      </v-col>
<v-col cols="12" xl="8" lg="8" md="8" class="d-flex justify-center">
            <p class="aboutText">
              As per Sudha’s saying, "Beauty is the illumination of your soul
              and Makeup is a tool meant to magnify the beauty that already
              exists inside. Sudha has been in this beauty industry for the
              past 10 years. After completing her post graduation in commerce,
              she had an unquenchable thirst for her passion towards the beauty
              industry."<br /><br />
              After graduating from AVINASHILINGAM UNIVERSITY with a good
              theoretical knowledge, she has offered her makeup services in
              several leading salons like Naturals, Green trends, Marria among
              other salons. She has completed her advanced makeup and hairstyle
              courses in Chennai. She has also taken additional certified master
              class in professional makeup with BLUSH BEAUTY BEYOND & SANGEETHA
              MAKEOVER ARTISTRY and has exposure to huge array of makeup
              techniques. These qualifications make her very versatile and can
              adapt to various makeup styles on the fly based on face types and
              occasions and has led her to provide makeup services independently
              to her loyal clientele.
            </p>
      </v-col>
    </v-row>
  </v-row>
</template>
<style lang="scss">
@import '~/assets/variables.scss';
.about {
  background-color: $primary-color;
}
.aboutText {
  color: $text-color;
}
</style>
