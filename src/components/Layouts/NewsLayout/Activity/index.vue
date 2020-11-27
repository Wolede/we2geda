<template>
  <v-sheet class="py-10">
    <v-container>
      <v-row>
        <v-col cols="12" sm="12" md="3" class="d-flex flex-column">
          <v-sheet class="image mb-2" height="100%" min-height="150"></v-sheet>
          <v-sheet class="image mt-2" height="100%" min-height="150"></v-sheet>
        </v-col>
        <v-col cols="12" sm="12" md="6">
          <v-sheet min-height="350" class="fill-height image"> </v-sheet>
        </v-col>
        <v-col cols="12" sm="12" md="3" class="d-flex flex-column">
          <v-sheet class="image mb-2" height="100%" min-height="150"></v-sheet>
          <v-sheet class="image mt-2" height="100%" min-height="150"></v-sheet>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script>
export default {};
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
