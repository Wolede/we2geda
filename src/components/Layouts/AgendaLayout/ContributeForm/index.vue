<template>
  <v-sheet class="py-10" color="primary" dark>
    <v-container>
      <div class="text-h5 text-center mb-6">
        {{ title }}
      </div>

      <div class="text-center mt-8">
        <v-btn
          class="white primary--text"
          depressed
          x-large
          href="https://forms.google.com"
          target="_blank"
        >
          Contribute Idea
        </v-btn>
      </div>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      title: "I have contributed my Ideas for Change, Have you?"
    };
  }
};
</script>

<style></style>
