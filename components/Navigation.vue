<template>
  <nav>
    <v-navigation-drawer disable-resize-watcher v-model="drawer" app>
      <v-list-item>
        <v-list-item-content>
          <v-img :src="require('@/assets/logo/BHG-Logo_White.svg')"></v-img>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list dense nav>
        <v-list-item
          v-for="nav in navigation"
          :key="nav.title"
          :href="nav.link"
          link
        >
          <v-list-item-icon>
            <v-icon>{{ nav.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ nav.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar flat app>
      <v-container>
        <v-row>
          <div class="toolbar-container">
            <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
          </div>
          <v-toolbar-title
            style="cursor: pointer"
            @click="$router.push('/')"
            class="navTitle"
            ><span class="larger">B</span>LACK <span class="larger">H</span>ILLS
            <span class="larger">G</span>EAR</v-toolbar-title
          >

          <v-spacer></v-spacer>

          <v-toolbar-items class="toolbar-navigation">
            <v-btn href="/" text> Home </v-btn>
            <v-btn href="/store" text> Store </v-btn>
            <v-btn href="/about" text> About </v-btn>
            <v-btn href="/contact" text> Contact </v-btn>
          </v-toolbar-items>
        </v-row>
      </v-container>

      <div></div>
    </v-app-bar>
  </nav>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
    navigation: [
      { title: 'Home', icon: 'mdi-pistol', link: '/' },
      { title: 'Store', icon: 'mdi-storefront', link: '/store' },
      { title: 'About', icon: 'mdi-image-filter-hdr', link: '/about' },
      {
        title: 'Contact',
        icon: 'mdi-book-open-blank-variant',
        link: '/contact',
      },
    ],
  }),
}
</script>

<style scoped>
.navTitle {
  letter-spacing: 0.1em;
  font-weight: 600;
  padding-top: 2px;
  /*font-family: 'volkhov', serif !important; */
}
.larger {
  font-size: 130%;
}

@media screen and (min-width: 960px) {
  .toolbar-container {
    display: none;
  }
}

@media screen and (max-width: 960px) {
  .toolbar-navigation {
    display: none;
  }
  .navTitle {
    display: none;
  }
  #app > div > nav > header {
    color: rgba(0, 0, 0, 0) !important;
    background-color: rgba(0, 0, 0, 0) !important;
  }
}
</style>
