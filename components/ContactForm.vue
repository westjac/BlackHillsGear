<template>
  <v-form
    name="contactUs"
    ref="form"
    v-model="valid"
    method="POST"
    data-netlify="true"
  >
    <input type="hidden" name="form-name" value="contactUs" />
    <v-text-field
      solo
      v-model="name"
      name="Name"
      label="Name"
      required
    ></v-text-field>
    <v-text-field
      solo
      v-model="email"
      name="Email"
      label="Email"
      required
    ></v-text-field>
    <v-text-field
      solo
      v-model="cellPhone"
      name="Cell Phone"
      label="Cell Phone"
      required
    ></v-text-field>
    <v-textarea
      solo
      name="Message"
      label="Message"
      v-model="message"
    ></v-textarea>
    <v-btn class="mr-4" type="submit" :disabled="false"> submit </v-btn>
  </v-form>
</template>

<script>
export default {
  data: () => ({
    valid: false,
    name: '',
    email: '',
    cellPhone: '',
    message: '',
  }),
}
</script>
