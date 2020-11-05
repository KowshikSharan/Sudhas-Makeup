<template>
  <v-app> 
    <v-main>
      <v-container fluid class="pa-0 cont">
          <MenuBar />
        <nuxt />
        <Footer />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
   components: {
    MenuBar,
    Footer
  },
  data () {
    return {
    }
  }
}
import MenuBar from '@/components/MenuBar.vue'
import Footer from '@/components/Footer.vue'
</script>
<style lang="scss">
@import '~/assets/variables.scss';
.cont {
  background-color: $secondary-color;
}
</style>
