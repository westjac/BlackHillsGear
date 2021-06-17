<template>
  <div>
    <v-carousel
      hide-delimiters
      :show-arrows="false"
      :continuous="true"
      :cycle="true"
    >
      <v-carousel-item
        class="darkened-image"
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
      ></v-carousel-item>
    </v-carousel>
    <v-img
      class="logo"
      style="margin-top: -25em"
      height="300px"
      contain
      src="/BHG-Logo_White.svg"
    ></v-img>
  </div>
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

<style scoped>
.darkened-image {
  filter: brightness(20%);
}
.logo {
  filter: drop-shadow(0px 3px 10px rgba(0, 0, 0, 1));
}
</style>
