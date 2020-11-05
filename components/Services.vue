<template>
  <v-row class="pa-2">
    <v-col cols="12" class="d-flex justify-center">
      <h1 class="text" id="services">Services</h1>
    </v-col>
    <v-col  cols="12" xl="6" lg="6" md="6" v-for="(item, i) in items" :key="i">

    <v-row class="card" >
      <v-col
        cols="12"
        xl="3"
        lg="3"
        md="3"
        sm="3"
        xs="3"
        class="d-flex justify-center "
      >
        <v-img
          width="300px"
          contain
          :src="item.src"
        />
      </v-col>
      <v-col
        cols="12"
        xl="9"
        lg="9"
        md="9"
        sm="9"
        xs="9"
        class="d-flex flex-column align-center align-xl-start align-lg-start align-md-start"
      >
        <h3 class="text">{{item.title}}</h3>
        <p class="text" align="justify">
         {{item.description}}
        </p>
      </v-col>
    </v-row>
</v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    items: [
      {
        src: require('../assets/images/model.png'),
        title: 'Model Photoshoot',
        description:
          'All kinds of traditional, western and bridal modelshoot is undertaken',
      },
      {
        src: require('../assets/images/bridal.png'),
        title: 'Bridal Makeup',
        description:
          'May ones love continue to grow everyday starting with a special day.Choose our makeup services to make the day extra special. Makeup services for marriages and receptions are undertaken.',
      },
      {
        src: require('../assets/images/hd.png'),
        title: 'HD|3D Makeup',
        description:
          'HD and 3D makeup is where we contour and soften your look to give a more refined makeover.',
      },
      {
        src: require('../assets/images/hairstyle.png'),
        title: 'Hair Styling and Hair Do',
        description:
          'Accentuate your look by dressing your hair like a medieval princess or like a modern go-getter. We provide hair dressing services for all occasions.',
      },
      {
        src: require('../assets/images/home.png'),
        title: 'Home Makeup Sevices',
        description:
          'Glam yourself up at the comfort of your home with our home makeup services.',
      },
      {
        src: require('../assets/images/class.png'),
        title: 'Makeup Classes',
        description:
          'Learn more on how to do makeups and hairstyles professionally with Sudhas makeup classes',
      },
    ],
  }),
}
</script>

<style lang="scss">
@import '~/assets/variables.scss';
.card {
  background-color: $primary-color;
  margin: 10px;
  border-radius: 10px;
}
.text {
  color: $text-color;
}
</style>
