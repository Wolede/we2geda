<template>
  <v-sheet outlined>
    <v-container fluid class="py-0">
      <v-sheet>
        <v-row>
          <v-col cols="12" sm="12" md="8" class="py-10 fill-height">
            <v-sheet :class="[$vuetify.breakpoint.smAndUp ? 'mx-10' : 'ml-3']">
              <div
                class="mb-6"
                :class="[$vuetify.breakpoint.smAndUp ? 'text-h2' : 'text-h3']"
              >
                {{ title }}
              </div>
              <ul>
                <li
                  class="text-subtitle-2 mb-4"
                  v-for="(desc, i) in descriptions"
                  :key="i"
                >
                  {{ desc }}
                </li>
              </ul>
            </v-sheet>
          </v-col>
          <v-col cols="12" sm="12" md="4" class="image">
            <v-sheet
              min-height="300"
              color="transparent"
              class="fill-height"
            ></v-sheet>
          </v-col>
        </v-row>
      </v-sheet>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      title: "Mission",
      descriptions: [
        "To ensure a secure, prosperous and united Nigeria through the peaceful transference of power led by capable leaders to lead Nigeria to become a 21st century economy.",
        "To galvanise political participation and demystify the flaws in the system including money-politics, godfatherism etc.          ",
        "To leverage the strength of our young people with a view to increase their patriotism and commitment for Project-Nigeria; the firm belief that a re-invented Nigeria is possible."
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.image {
  background-image: url("/images/mission.jpg");
  background-color: rgba($color: $light-grey, $alpha: 0.65);
  //   background-color: rgba($color: $dark-grey, $alpha: 0.8);
  background-position: center center;
  background-repeat: no-repeat;
  background-blend-mode: hue;
  background-size: cover;
}
</style>
