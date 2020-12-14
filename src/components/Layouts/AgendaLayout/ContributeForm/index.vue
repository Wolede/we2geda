<template>
  <v-sheet class="py-10" color="primary" dark>
    <v-container>
      <div class="text-h5 text-center mb-6">
        {{ title }}
      </div>

      <div class="text-center mt-8">
        <v-form @submit.prevent="onSubmit">
            <v-row>
              <v-col
                cols="12"
                md="4"
              >
                <v-text-field
                  v-model="name"
                  label="Name"
                  required
                ></v-text-field>
              </v-col>

              <v-col
                cols="12"
                md="4"
              >
                <v-text-field
                  v-model="phone"
                  label="Phone"
                  type="tel"
                  required
                ></v-text-field>
              </v-col>

              <v-col
                cols="12"
                md="4"
              >
                <v-text-field
                  v-model="email"
                  label="Email"
                  type="email"
                  required
                ></v-text-field>
              </v-col>
              <v-col
                cols="12"
                md="4"
              >
                <v-text-field
                  v-model="location"
                  label="Country"
                  required
                ></v-text-field>
              </v-col>
              <v-col
                cols="12"
                md="4"
              >
                <v-text-field
                  v-model="area"
                  label="State of Residency"
                  required
                ></v-text-field>
              </v-col>
              <v-col
                cols="12"
                md="4"
              >
                <v-file-input
                  v-model="attachment"
                  label="Polling Unit Code"
                  counter
                  show-size
                  chips
                  required
                ></v-file-input>
              </v-col>
            </v-row>
            <div>
              <v-btn
                class="white primary--text"
                depressed
                x-large
                type="submit"
              >
                Add Mine
              </v-btn>

            </div>
        </v-form>
      </div>
    </v-container>
  </v-sheet>
</template> 

<script>
export default {
  data() {
    return {
      title: "I have contributed my Ideas for Change, Have you?",
      name: '',
      phone: '',
      email: '',
      location: '',
      area: '',
      attachment: null
    };
  },
  methods: {
    onSubmit() {
      //do something
    }
  },
};
</script>

<style></style>
