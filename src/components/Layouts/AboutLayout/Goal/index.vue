<template>
  <v-sheet color="accent" class="py-10" dark>
    <v-container>
      <v-sheet class="mx-auto" max-width="1000" color="transparent">
        <div
          class="mb-8"
          :class="[$vuetify.breakpoint.smAndUp ? 'text-h2' : 'text-h4']"
        >
          {{ title1 }}
        </div>
        <div class="text-subtitle-2">
          {{ description1 }}
        </div>
        <v-divider
          class="my-15"
          style="border-width: initial;border-color:white"
        ></v-divider>
        <div
          class="mb-8"
          :class="[$vuetify.breakpoint.smAndUp ? 'text-h2' : 'text-h4']"
        >
          {{ title2 }}
        </div>
        <div class="text-subtitle-2">
          {{ description2 }}
        </div>
      </v-sheet>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      title1: "Organising works — and it has the power to change history.",
      description1:
        "With over 36 State chapters around the country, We2Geda is building an inclusive movement from the grassroots up, community by community, one conversation at a time—whether it is at the marketplace, place of worship, or on your mobile phone.",
      title2: "Our Goal",
      description2:
        "To create a new generation of patriotic competent leaders to lead Nigeria to become a 21st century economy."
    };
  }
};
</script>

<style></style>
