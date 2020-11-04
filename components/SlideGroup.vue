<template>
            <v-slide-group v-model="model" class="pa-6" show-arrows="true" continuous="true">
          <v-slide-item v-for="n in 13" :key="n">
            <v-card flat tile height="400" width="300" class= "shade">
              <v-img
                :src="require(`@/assets/images/${n}.png`)"
                :lazy-src="require(`@/assets/images/${n}.png`)"
                aspect-ratio="0.67"
                class="black"
                @click.stop="dialogfn(require(`@/assets/images/${n}.png`))"
              >
                <template v-slot:placeholder>
                  <v-row class="fill-height ma-0" align="center" justify="center">
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
.shade{
  border-style:solid;
  border-width: 10px;

}
</style>
