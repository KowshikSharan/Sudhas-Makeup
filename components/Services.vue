<template>
  <v-row class="ma-5 d-flex justify-center">
      <v-col cols="12" class="d-flex justify-center">
    <h1 id="services">Services</h1>
      </v-col>
    <v-row class="card">
      <v-col
        cols="12"
        xl="3"
        lg="3"
        md="3"
        class="d-flex justify-start justify-sm-center"
      >
        <v-img
          max-width="200px"
          contain
          :src="require('../assets/images/model.png')"
        />
      </v-col>
      <v-col
        cols="12"
        xl="9"
        lg="9"
        md="9"
        class="d-flex justify-end justify-sm-center"
      >
        <p>
          Model Photoshoot All kinds of traditional, western and bridal model
          shoot is undertaken
        </p>
      </v-col>
    </v-row>
    <v-row class="card">
      <v-col>
        <v-img
          :src="require('../assets/images/bridal.png')"
          max-width="200px"
          contain
        ></v-img>
      </v-col>
      <v-col>
        Bridal Makeup May one's love continue to grow everyday starting with a
        special day.Choose our makeup services to make the day extra special.
        Makeup services for marriages and receptions are undertaken.
      </v-col>
    </v-row>
    <v-row class="card">
      <v-col>
        <v-img
          :src="require('../assets/images/hd.png')"
          contain
          max-width="200px"
        ></v-img>
      </v-col>
      <v-col>
        HD|3D Makeup HD and 3D makeup is where we contour and soften your look
        to give a more refined makeover.
      </v-col>
    </v-row>
    <v-row class="card">
      <v-col>
        <v-img
          :src="require('../assets/images/hairstyle.png')"
          contain
          max-width="200px"
        ></v-img>
      </v-col>
      <v-col>
        Hair Styling and Hair Do's Accentuate your look by dressing your hair
        like a medieval princess or like a modern go-getter. We provide hair
        dressing services for all occasions.
      </v-col>
    </v-row>
    <v-row class="card">
      <v-col>
        <v-img :src="require('../assets/images/home.png')" contain
          max-width="200px"></v-img> </v-col
      ><v-col>
        Home Makeup Sevices Glam yourself up at the comfort of your home with
        our home makeup services.
      </v-col>
    </v-row>
    <v-row class="card">
      <v-col>
        <v-img :src="require('../assets/images/class.png')" contain
          max-width="200px"></v-img> </v-col
      ><v-col>
        Makeup Classes Learn more on how to do makeups and hairstyles
        professionally with Sudha's makeup classes
      </v-col>
    </v-row>
  </v-row>
</template>
<style>
.card {
    background-color:#272727;
    margin: 10px;
}
</style>