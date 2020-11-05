<template>
            <v-slide-group class="pa-6 slider" :show-arrows="true" continuous="true">
          <v-slide-item class="slider" v-for="n in 13" :key="n">
            <v-card color="#FEEAE6" flat tile height="400" width="300" class= "shade">
              <v-img
                :src="require(`@/assets/images/${n}.jpg`)"
                :lazy-src="require(`@/assets/images/${n}.jpg`)"
                aspect-ratio="0.67"
                class="slider"
                @click.stop="dialogfn(require(`@/assets/images/${n}.jpg`))"
              >
                <template v-slot:placeholder>
                  <v-row class="fill-height ma-0 slider" align="center" justify="center">
                    <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
                  </v-row>
                </template>
              </v-img>
              <v-row>
                <v-dialog
                  v-model="dialog"
                  max-width="500"
                  :scrollable='false'
                  overlay-opacity ="0.15"

                >
                  <v-img :src="selectedImage" alt width="100%" contain />
                </v-dialog>
              </v-row>
            </v-card>
          </v-slide-item>
        </v-slide-group>
</template>
<script>
export default {
     props: {
    source: String
  },
  data: () => ({
    selectedImage: null,
    drawer: false,
    dialog: false
  }),
  methods: {
    dialogfn(src) {
      console.log("Zoom", src);
      this.selectedImage = src;
      this.dialog = true;
    }
  }
}
</script>
<style lang="scss">
@import '~/assets/variables.scss';
.shade{
  border-style:solid;
  border-width: 10px;
  background-color: $secondary-color;
}
.slider {
  background-color: $secondary-color;
}
</style>
