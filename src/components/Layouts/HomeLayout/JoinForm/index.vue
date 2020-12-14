<template>
  <v-sheet class="py-10" color="primary" dark>
    <v-container>
      <div class="text-h4 text-center mb-6">
        {{ title }}
      </div>
      <v-sheet
        class="body-2 text-center mx-auto"
        v-for="(desc, i) in descriptions"
        :key="i"
        max-width="500"
        color="transparent"
      >
        {{ desc }}
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
                class="white primary--text"
                depressed
                x-large
                type="submit"
              >
                Count Me In
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
      title: "Join the Action",
      descriptions: [
        "Nigeria needs you now more than ever. Join this united tribe of people morally committed to a better Nigeria.",
        "Come Onboard, Let us Walk the Talk:"
      ],
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
