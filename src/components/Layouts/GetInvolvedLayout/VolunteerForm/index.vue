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
        <v-btn
          depressed
          color="primary"
          x-large
          href="https://forms.google.com"
          target="_blank"
        >
          I'm in - Let's Do This!
        </v-btn>
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
        "A Nation divided cannot stand; any intent of division is a threat to our existence. Enough of the talks, let’s come together and channel our passion into action.",
      description2:
        "Enough of the talks, let's come together and channel our passion into action"
    };
  }
};
</script>

<style></style>
