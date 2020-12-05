<template>
  <v-sheet dark class="join-highlight py-10">
    <v-container>
      <v-row align="center">
        <v-col cols="12" sm="12" md="6">
          <div class="fill-height">
            <div class="text-h4 mb-6">
              {{ title }}
            </div>
            <div class="text-body-2">
              {{ description }}
            </div>
            <v-btn
              depressed
              x-large
              class="transparent accent--text pl-0 mt-10"
              to="/about"
              nuxt
            >
              <span class="text-decoration-underline">
                The time to act is now
              </span>
              <v-icon right>
                mdi-arrow-right
              </v-icon>
            </v-btn>
          </div>
        </v-col>
        <v-col cols="12" sm="12" md="6">
          <div class="fill-height pa-4">
            <v-sheet
              class="mx-auto pa-8"
              rounded
              color="white"
              width="100%"
              max-width="350"
              light
            >
              <v-img
                src="https://picsum.photos/id/11/500/300"
                height="180"
                width="180"
                style="border-radius:50%"
                class="mx-auto mb-6"
              >
              </v-img>
              <div class="text-h5">
                {{ name }}
              </div>
              <div class="text-body-1 mb-6">
                {{ school }}
              </div>
              <div class="text-body-2">
                {{ bio }}
              </div>
              <v-btn
                depressed
                x-large
                class="transparent accent--text pl-0 mt-6"
                to="/about"
                nuxt
              >
                <span class="text-decoration-underline">
                  Join Us
                </span>
                <v-icon right>
                  mdi-arrow-right
                </v-icon>
              </v-btn>
            </v-sheet>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      title: "We are mentoring tomorrow’s leaders today.",
      description:
        "We are dedicated to discovering, mentoring, and training the next generation of patriotic leaders, providing them with a competency based-model for leadership development required to drive the much-needed change of the Nigerian State and to make a lasting difference in nation-building.",
      name: "Musa Uche",
      school: "University of Lagos",
      bio:
        "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat inventore nihil corrupti, nemo unde quibusdam? Quia, dolore alias. Eaque suscipit a iusto modi nobis unde consequuntur quisquam ab, reprehenderit vel!"
    };
  }
};
</script>

<style lang="scss" scoped>
.join-highlight {
  padding-top: 120px;
  background-image: url("/images/home-two.jpg");
  background-color: rgba($color: $dark-grey, $alpha: 0.85);
  //   background-color: rgba($color: $dark-grey, $alpha: 0.8);
  background-position: center center;
  background-repeat: no-repeat;
  background-blend-mode: hue;
  background-size: cover;
}
</style>
