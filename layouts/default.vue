<template>
  <v-app>
    <Navigation />
    <v-main>
      <!--<v-alert dense outlined prominent text dismissible type="warning"
        >Orders will be delayed till February 15th. Sorry for the inconvenience.
      </v-alert>-->
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
