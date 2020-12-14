<template>
  <div>
    <div
    class="mt-10 mb-8"
    :class="[$vuetify.breakpoint.smAndUp ? 'text-h2' : 'text-h4']"
    >
      {{ title }}
    </div>
    <div class="text-right mt-8">
      <v-form @submit.prevent="onSubmit">
        <v-row>
          <v-col
            cols="12"
            md="6"
          >
            <v-text-field
              v-model="name"
              label="Name"
              outlined
              hide-details
              required
            ></v-text-field>
          </v-col>

          <v-col
            cols="12"
            md="6"
          >
            <v-text-field
              v-model="subject"
              label="Subject"
              outlined
              hide-details
              required
            ></v-text-field>
          </v-col>

          <v-col
            cols="12"
            md="6"
          >
            <v-text-field
              v-model="phone"
              label="Phone"
              type="tel"
              outlined
              hide-details
              required
            ></v-text-field>
          </v-col>

          <v-col
            cols="12"
            md="6"
          >
            <v-text-field
              v-model="email"
              label="Email"
              type="email"
              outlined
              hide-details
              required
            ></v-text-field>
          </v-col>
          <v-col
            cols="12"
            md="12"
          >
            <v-textarea
              v-model="message"
              label="Message"
              outlined
              hide-details
              required
            ></v-textarea>
          </v-col>
        </v-row>
        <div class="mt-6">
          <v-btn
            class="primary"
            depressed
            x-large
            type="submit"
          >
            Send
          </v-btn>
        </div>
      </v-form>
    </div>
  </div>
</template>

<script>
export default {
data() {
  return {
    title: 'Contact Us',
    name: '',
    subject: '',
    phone: '',
    email: '',
    message: '',
  }
},
methods: {
    onSubmit() {
      //do something
    }
  },
}
</script>

<style>

</style>