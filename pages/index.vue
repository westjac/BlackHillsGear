/* eslint-disable */
<template>
  <main>
    <v-row justify="center">
      <v-col>
        <Megatron />
      </v-col>
    </v-row>
    <v-container my-4>
      <v-row justify="center">
        <v-col :xs="8" :sm="4">
          <h1 class="title">Post Your Pics!</h1>
          <br />
          <p>
            Share your pictures of your Black Hills Gear with us and we might
            just share them on the web! Use the hashtag #BlackHillsGear! By
            sending us photos, you agree to let us post them for advertizing
            purposes.
          </p>
        </v-col>
        <v-col :xs="8" :sm="6">
          <v-img
            height="80%"
            :src="require('@/assets/img/bestgun.jpg')"
          ></v-img>
        </v-col>
      </v-row>
      <div style="height: 100px"></div>
    </v-container>
  </main>
</template>

<script>
export default {
  head() {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' },
      ],
    }
  },
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
/* eslint-disable */
