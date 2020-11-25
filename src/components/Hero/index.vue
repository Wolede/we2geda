<template>
  <v-sheet
    class="hero almost-fill-screen"
    :style="`background-image: url(images/${backgroundImage})`"
    dark
    id="below-hero"
  >
    <v-container class="fill-height">
      <v-row justify="center">
        <v-sheet
          max-width="1000"
          color="transparent"
          class="d-flex justify-center"
        >
          <div
            class="text-center text-uppercase"
            :class="[$vuetify.breakpoint.smAndUp ? 'text-h1' : 'text-h4']"
            v-if="page === 'home'"
          >
            You Can Be The <span class="primary--text"> Change. </span>
          </div>
        </v-sheet>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  props: {
    page: {
      type: String
    },
    backgroundImage: {
      type: String
    }
  },
  data() {
    return {
      title: "You Can Be The Change"
    };
  }
};
</script>

<style lang="scss" scoped>
.hero {
  padding-top: 120px;
  background-color: rgba($color: $light-grey, $alpha: 0.65);
  //   background-color: rgba($color: $dark-grey, $alpha: 0.8);
  background-position: center center;
  background-repeat: no-repeat;
  background-blend-mode: hue;
  background-size: cover;
}
.almost-fill-screen {
  min-height: 530px;
  height: 80vh;
  @media screen and (min-width: 960px) {
    height: calc(100vh - 120px);
  }
  @media screen and (min-width: 1424px) {
    height: calc(100vh - 200px);
  }
}
</style>
