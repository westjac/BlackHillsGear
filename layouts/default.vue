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
html,
body {
  overflow-x: hidden;
}
body {
  position: relative;
}
</style>
