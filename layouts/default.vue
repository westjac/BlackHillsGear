<template>
  <v-app>
    <Navigation />
    <v-main>
      <v-alert dense outlined prominent text dismissible type="warning"
        >Begining January 25th no custom orders will be processed until April.
        Although, we do have some various colors and sizes available for
        immediate shipping during this time frame. Please contact us for more
        information. Sorry for the inconvenience.
      </v-alert>
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
