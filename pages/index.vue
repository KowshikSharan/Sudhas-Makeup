<template>
<div class="pa-0 mb-50">
      <v-row>
        <v-col cols="12" class="d-flex flex-wrap justify-center">
          <h1 class="portfolio" id="portfolio">Portfolio</h1>
        </v-col>
      </v-row>
      <v-row class="slider">
        <SlideGroup />
      </v-row>

      <About />
      <Services />
      </div>
</template>
<script>
export default {
  components: {
    SlideGroup,
    About,
    Services
  },
}
import SlideGroup from '@/components/SlideGroup.vue'
import About from '@/components/About.vue'
import Services from '@/components/Services.vue'
</script>
<style lang="scss">
@import '~/assets/variables.scss';
.about {
  text-align: justify;
}
.portfolio {
  color: $text-color;
}
.empty {
width: 1000px;
background-color: $primary-color;
}
.content {
  background-color: $primary-color;
}
.slider {
  background-color: $secondary-color;
}
</style>