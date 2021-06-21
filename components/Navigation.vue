<template>
  <v-app-bar flat app>
    <v-container>
      <v-row>
        <v-toolbar-title
          style="cursor: pointer"
          @click="$router.push('/')"
          class="navTitle"
          ><span class="larger">B</span>LACK <span class="larger">H</span>ILLS
          <span class="larger">G</span>EAR</v-toolbar-title
        >

        <v-spacer></v-spacer>

        <v-toolbar-items>
          <v-btn href="/" text> Home </v-btn>
          <v-btn href="/store" text> Store </v-btn>
          <v-btn href="/about" text> About </v-btn>
          <v-btn href="/contact" text> Contact </v-btn>
        </v-toolbar-items>
      </v-row>
    </v-container>

    <div></div>
  </v-app-bar>
</template>

<style scoped>
.navTitle {
  letter-spacing: 0.1em;
  font-weight: 600;
  /*font-family: 'volkhov', serif !important; */
}
.larger {
  font-size: 130%;
}
</style>
