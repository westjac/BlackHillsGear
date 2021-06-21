<template>
  <v-container>
    <v-row style="text-align: center">
      <v-col>
        <h1 class="header">Get in touch with us.</h1>
        <br />
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="6">
        <ContactForm />
      </v-col>
      <v-col>
        <v-img :src="require('@/assets/logo/BHG-Logo_White.svg')"></v-img>
        <br />
        <p class="contactText">
          Questions? Comments? Want to know more about our product? Shoot us a
          message and we will get back with you as fast as you can say "got
          'em!"
        </p></v-col
      >
    </v-row>
  </v-container>
</template>

<style scoped>
.contactText {
  font-size: 20px;
  text-align: center;
}
</style>
