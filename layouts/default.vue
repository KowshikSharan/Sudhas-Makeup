<template>
  <v-app dark> 
    <v-main>
      <v-container fluid class="pa-0">
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
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
import MenuBar from '@/components/MenuBar.vue'
import Footer from '@/components/Footer.vue'
</script>
