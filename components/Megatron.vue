<template>
  <div class="parent">
    <v-carousel
      hide-delimiters
      :show-arrows="false"
      :continuous="true"
      :cycle="true"
    >
      <v-carousel-item
        class="darkened-image"
        transition="fade-transition"
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
      ></v-carousel-item>
    </v-carousel>
    <img class="logo child" height="300px" src="/BHG-Logo_White.svg" />
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
.parent {
  display: grid;
  position: relative;
}
.child {
  max-width: 555px;
  max-height: 300px;
  width: auto;
  height: auto;
  position: absolute;
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}
</style>
