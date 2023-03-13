<template>
  <v-app>
    <Navigation />
    <v-main>
      <v-alert dense outlined prominent text dismissible type="warning"
        >Currently away and will process orders in the first week in April. Thanks
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
