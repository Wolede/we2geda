<template>
  <v-sheet class="py-10">
    <v-container>
      <div class="text-h4 text-center mb-6">
        {{ title }}
      </div>
      <v-sheet class="body-2 text-center mx-auto" max-width="500">
        {{ description }}
      </v-sheet>
      <div class="text-center mt-8">
        <v-btn
          depressed
          color="secondary"
          x-large
          href="https://we2geda.tk"
          target="_blank"
        >
          Join Us
        </v-btn>
      </div>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      title: "The Time To Act is Now",
      description:
        "We2geda leaders and partners across the country are making a difference in their communities through the determined and steady work of organising."
    };
  }
};
</script>

<style></style>
