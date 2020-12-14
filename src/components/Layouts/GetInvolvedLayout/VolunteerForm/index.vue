<template>
  <v-sheet class="py-10">
    <v-container>
      <div class="text-h4 text-center mb-6">
        {{ title }} 
      </div>
      <v-sheet class="text-h6 text-center mx-auto mb-4" max-width="1000">
        {{ description }}
      </v-sheet>
      <v-sheet
        class="text-h6 text-center mx-auto primary--text"
        max-width="1000"
      >
        {{ description2 }}
      </v-sheet>
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
                  v-model="country"
                  label="Country"
                  required
                ></v-text-field>
              </v-col>
              <v-col
                cols="12"
                md="4"
              >
                <v-text-field
                  v-model="state"
                  label="State of Residency"
                  required
                ></v-text-field>
              </v-col>
              <v-col
                cols="12"
                md="4"
              >
                <v-text-field
                  v-model="unitCode"
                  label="Polling Unit Code"
                  required
                ></v-text-field>
              </v-col>
            </v-row>
            <div>
              <v-btn
                class="primary"
                depressed
                x-large
                type="submit"
              >
                I'm in - Let's Do This!
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
      title: "Become a Volunteer",
      description:
        "A Nation divided cannot stand; any intent of division is a threat to our existence.",
      description2:
        "Enough of the talks, let's come together and channel our passion into action",
        name: '',
      phone: '',
      email: '',
      country: '',
      state: '',
      unitCode: ''
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
