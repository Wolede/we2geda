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
        <v-btn
          class="white primary--text"
          depressed
          x-large
          href="https://forms.google.com"
          target="_blank"
        >
          Count Me In
        </v-btn>
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
      ]
    };
  }
};
</script>

<style></style>
