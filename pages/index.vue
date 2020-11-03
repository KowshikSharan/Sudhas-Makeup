<template>
  <v-app id="inspire">
    <v-app-bar app clipped-left>
      
      <v-row justify="start">
      <v-toolbar-title > <v-img :src="require('../assets/images/logo.png')" height="60px" contain></v-img></v-toolbar-title>
</v-row>
<v-row justify="space-around">
        <v-btn depressed x-large href="#about">About</v-btn>
        <v-btn depressed x-large href="#portfolio">Portfolio</v-btn>
        <v-btn depressed x-large href="#services">Services</v-btn>
      </v-row>
    </v-app-bar>

    <v-content>
      <v-container class="fill-height" fluid>
        <div>
                <h1 id = "portfolio">Portfolio</h1>
                </div>

       <slidegroup/>

        <v-divider></v-divider>
        <h1 id="about">About</h1>
        <v-row>
          <v-col cols="12">
            <v-card >
              <div class="d-flex flex-no-wrap justify-start">
                <v-avatar class="ma-3" size = "250" tile>
                  <v-img :src="require('../assets/images/about.png')" contain></v-img>
                </v-avatar>
                <div>
                  <v-card-title  class="display-1">About</v-card-title>

                  <v-card-subtitle class="title"><p class = "about">As per Sudha’s saying, "Beauty is the illumination of your soul and Makeup is a tool meant to magnify the beauty that already exists inside".
Sudha has been in this beauty industry for the past 10 years. After completing her post graduation in commerce, she had an unquenchable thirst for her passion towards the beauty industry.<br><br>
After graduating from AVINASHILINGAM UNIVERSITY with a good theoretical knowledge, she has offered her makeup services in several leading salons like Naturals, Green trends, Marria among other salons. She has completed her advanced makeup and hairstyle courses in Chennai. She has also taken additional certified master class in professional makeup with BLUSH BEAUTY BEYOND & SANGEETHA MAKEOVER ARTISTRY and has exposure to huge array of makeup techniques. 
These qualifications make her very versatile and can adapt to various makeup styles on the fly based on face types and occasions and has led her to provide makeup services independently to her loyal clientele. </p> 
</v-card-subtitle>
                </div>
              </div>
            </v-card>
          </v-col>
        </v-row>

        <h1 id="services">Services</h1>
        <v-row justify="space-around">
          <v-col cols="12">
            <v-card >
              <div class="d-flex flex-no-wrap justify-start">
                <v-avatar class="ma-3" height="300" width="200" tile>
                  <v-img :src="require('../assets/images/model.png')"></v-img>
                </v-avatar>
                <div>
                  <v-card-title class="display-1">Model Photoshoot</v-card-title>

                  <v-card-subtitle class="title">All kinds of traditional, western and bridal model shoot is undertaken</v-card-subtitle>
                </div>
              </div>
            </v-card>
          </v-col>
          <v-col cols="12">
            <v-card >
              <div class="d-flex flex-no-wrap justify-start">
                <v-avatar class="ma-3" height="300" width="200" tile>
                  <v-img :src="require('../assets/images/bridal.png' )" contain></v-img>
                </v-avatar>
                <div>
                  <v-card-title class="display-1">Bridal Makeup</v-card-title>

                  <v-card-subtitle
                    class="title"
                  >May one's love continue to grow everyday starting with a special day.Choose our makeup services to make the day extra special. Makeup services for marriages and receptions are undertaken.</v-card-subtitle>
                </div>
              </div>
            </v-card>
          </v-col>
          <v-col cols="12">
            <v-card >
              <div class="d-flex flex-no-wrap justify-start">
                <v-avatar class="ma-3" height="300" width="200" tile>
                  <v-img :src="require('../assets/images/hd.png')" contain></v-img>
                </v-avatar>
                <div>
                  <v-card-title class="display-1">HD|3D Makeup</v-card-title>

                  <v-card-subtitle class="title">HD and 3D makeup is where we contour and soften your look to give a more refined makeover.</v-card-subtitle>
                </div>
              </div>
            </v-card>
          </v-col>
          <v-col cols="12">
            <v-card >
              <div class="d-flex flex-no-wrap justify-start">
                <v-avatar class="ma-3" height="300" width="200" tile>
                  <v-img :src="require('../assets/images/hairstyle.png')" contain></v-img>
                </v-avatar>
                <div>
                  <v-card-title class="display-1">Hair Styling and Hair Do's</v-card-title>

                  <v-card-subtitle class="title">Accentuate your look by dressing your hair like a medieval princess or like a modern go-getter. We provide hair dressing services for all occasions.</v-card-subtitle>
                </div>
              </div>
            </v-card>
          </v-col>
          <v-col cols="12">
            <v-card >
              <div class="d-flex flex-no-wrap justify-start">
                <v-avatar class="ma-3" height="300" width="200" tile>
                  <v-img :src="require('../assets/images/home.png')" ></v-img>
                </v-avatar>
                <div>
                  <v-card-title class="display-1">Home Makeup Sevices</v-card-title>

                  <v-card-subtitle class="title">Glam yourself up at the comfort of your home with our home makeup services.</v-card-subtitle>
                </div>
              </div>
            </v-card>
          </v-col>
           <v-col cols="12">
            <v-card >
              <div class="d-flex flex-no-wrap justify-start">
                <v-avatar class="ma-3" height="300" width="200" tile>
                  <v-img :src="require('../assets/images/class.png')"></v-img>
                </v-avatar>
                <div>
                  <v-card-title class="display-1">Makeup Classes</v-card-title>

                  <v-card-subtitle class="title">Learn more on how to do makeups and hairstyles professionally with Sudha's makeup classes</v-card-subtitle>
                </div>
              </div>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>

    <v-footer app>
      <v-row justify="space-around">
        <v-btn href="https://www.instagram.com/sudha_makeover_artistry/?hl=en" target="blank">
          <v-icon x-large>mdi-instagram</v-icon>@sudha_makeover_artistry
        </v-btn>
        <div>
          <v-icon x-large>mdi-email</v-icon>sudharavishankar97851@gmail.com
        </div>
        <div>
          <v-icon large>mdi-cellphone</v-icon>+91 766 705 0279
        </div>
      </v-row>
    </v-footer>
  </v-app>
</template>
<script>
export default {
 
  components:{
    slidegroup
  },
  created() {
    this.$vuetify.theme.dark = true;
  }
};
import slidegroup from '@/components/SlideGroup.vue';

</script>
<style lang="scss">
.about{
text-align:justify
}
</style>