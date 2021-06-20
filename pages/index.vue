<template>
  <main>
    <v-row justify="center">
      <v-col>
        <Megatron />
      </v-col>
    </v-row>
    <v-container my-4>
      <v-row>
        <v-col cols="12">
          <v-card>
            <v-row>
              <v-col cols="6">
                <v-card-title class="title"> Post Your Pics! </v-card-title>
                <v-card-text>
                  Share your pictures of your Black Hills Gear with us and we
                  might just share them on the web! Use the hashtag
                  #BlackHillsGear on Facebook and Instagram! By sending us
                  photos, you agree to let us post them for advertizing
                  purposes.
                </v-card-text>
                <v-card-actions>
                  <v-btn justify="center" color="primary" text>
                    Send us your photos
                    <v-icon right dark> mdi-cloud-upload </v-icon>
                  </v-btn>
                </v-card-actions>
              </v-col>
              <v-col cols="6">
                <v-img
                  class="rounded-sm mr-3"
                  max-height="300"
                  src="/images/bestgun.jpg"
                ></v-img>
              </v-col>
            </v-row>
          </v-card>
          <div style="height: 300px"></div>
        </v-col>
      </v-row>
    </v-container>
  </main>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: '/images/bestgun.jpg',
        },
        {
          src: '/images/truckgun.jpg',
        },
      ],
    }
  },
}
</script>
