<template>
  <v-footer color="lighten-1">
    <v-row justify="center" no-gutters>
      <v-btn
        v-for="act in socialMedias"
        :key="act.icon"
        :href="act.link"
        target="_blank"
        class="mx-4 white--text"
        icon
      >
        <v-icon size="24px">
          {{ act.icon }}
        </v-icon>
      </v-btn>
      <v-col class="lighten-4 py-4 text-center white--text" cols="12">
        {{ new Date().getFullYear() }} — <strong>Black Hills Gear</strong>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    socialMedias: [
      {
        icon: 'mdi-facebook',
        link: 'https://www.facebook.com/BlackHillsGear/',
      },
      {
        icon: 'mdi-instagram',
        link: 'https://www.facebook.com/BlackHillsGear/',
      },
    ],
  }),
}
</script>
