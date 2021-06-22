<template>
  <div class="parent">
    <v-carousel
      class="megatron"
      hide-delimiters
      :show-arrows="false"
      :continuous="true"
      :cycle="true"
    >
      <v-carousel-item
        class="darkened-image"
        :src="require('@/assets/img/bestgun.jpg')"
      ></v-carousel-item>
      <v-carousel-item
        class="darkened-image"
        :src="require('@/assets/img/truckgun.jpg')"
      ></v-carousel-item>
    </v-carousel>
    <img
      class="logo child"
      height="300px"
      :src="require('@/assets/logo/BHG-Logo_White.svg')"
    />
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style scoped>
.darkened-image {
  filter: brightness(20%);
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
  top: 2em;
  left: 0;
  bottom: 0;
  right: 0;
}

@media screen and (max-width: 960px) {
  .megatron {
    height: 360px !important;
  }
}
</style>
