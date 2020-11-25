<template>
  <v-sheet class="py-10">
    <v-container>
      <v-row align="center">
        <v-col cols="12" sm="12" md="6" class="fill-height">
          <div class="text-h4" v-for="(title, i) in titles" :key="i">
            {{ title }}
          </div>
          <v-btn
            depressed
            x-large
            class="transparent accent--text pl-0 mt-6"
            to="/about"
            nuxt
          >
            <span class="text-decoration-underline">
              Find out more
            </span>
            <v-icon right>
              mdi-arrow-right
            </v-icon>
          </v-btn>
        </v-col>
        <v-col cols="12" sm="12" md="6" class="fill-height">
          <div
            class="d-flex flex-column align-center justify-center fill-height"
          >
            <div
              class="text-body-2 mb-15"
              v-for="(desc, i) in descriptions"
              :key="i"
            >
              {{ desc }}
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  name: "HomeAbout",
  data() {
    return {
      titles: ["We Respect.", "We Empower.", "We Unify.", "We Act."],
      descriptions: [
        "WE2GEDA is committed to unifying and mobilizing patriotic Nigerians from all walks of life. For the change we desire; we must come together, think together, move together, and act together — it requires people like you.",
        "With fellow compatriots in Nigeria, Africa, and across the world, WE2GEDA aims to build this movement from the ground up, person to person, community by community—because democracy isn’t a thought rather it is an act. Get Involved!"
      ]
    };
  }
};
</script>

<style></style>
