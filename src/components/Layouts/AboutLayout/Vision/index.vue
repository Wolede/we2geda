<template>
  <v-sheet outlined>
    <v-container fluid class="py-0">
      <v-sheet>
        <v-row>
          <v-col cols="12" sm="12" md="6" class="image">
            <v-sheet
              min-height="300"
              color="transparent"
              class="fill-height"
            ></v-sheet>
          </v-col>
          <v-col cols="12" sm="12" md="6" class="py-10 fill-height">
            <v-sheet
              :class="[$vuetify.breakpoint.smAndUp ? 'ml-10' : 'ml-3']"
              max-width="500"
            >
              <div
                class="mb-6"
                :class="[$vuetify.breakpoint.smAndUp ? 'text-h2' : 'text-h3']"
              >
                {{ title }}
              </div>
              <div class="text-subtitle-2">
                {{ description }}
              </div>
            </v-sheet>
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
      title: "Vision",
      description:
        "To harness democratic partnerships and technology to unify Nigerians all over the world to actualize a free, peaceful, and prosperous nation."
    };
  }
};
</script>

<style lang="scss" scoped>
.image {
  background-image: url("/images/puzzle.jpg");
  background-color: rgba($color: $light-grey, $alpha: 0.65);
  //   background-color: rgba($color: $dark-grey, $alpha: 0.8);
  background-position: center center;
  background-repeat: no-repeat;
  background-blend-mode: hue;
  background-size: cover;
}
</style>
