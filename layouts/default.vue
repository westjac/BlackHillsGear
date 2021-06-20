<template>
  <v-app>
    <Navigation />
    <v-main>
      <nuxt id="siteContent" />
    </v-main>
    <Footer />
  </v-app>
</template>

<style>
.v-application {
  font-family: 'Chivo', sans-serif !important;
}
.v-application .title {
  font-family: 'Volkhov', serif !important;
  font-weight: 700;
  font-size: 2.5rem !important;
}
</style>
