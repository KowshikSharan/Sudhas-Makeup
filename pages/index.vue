<template>
<div class="pa-0">
      <v-row>
        <v-col cols="12" class="d-flex flex-wrap justify-center">
          <h1 id="portfolio">Portfolio</h1>
        </v-col>
      </v-row>
      <v-row>
        <SlideGroup />
      </v-row>

      <About />
      <Services />
      <v-row>
        <v-col class="d-flex empty"></v-col>
      </v-row>
      </div>
</template>
<script>
export default {
  components: {
    SlideGroup,
    About,
    Services
  },
  created() {
    this.$vuetify.theme.dark = true
  },
}
import SlideGroup from '@/components/SlideGroup.vue'
import About from '@/components/About.vue'
import Services from '@/components/ServicesLoop.vue'
</script>
<style lang="scss">
.about {
  text-align: justify;
}
.empty {
width: 1000px;
background-color: hotpink;
}
.content {
  background-color: hotpink;
}
</style>