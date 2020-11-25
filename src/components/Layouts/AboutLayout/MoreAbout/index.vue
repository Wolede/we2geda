<template>
  <v-sheet class="py-10">
    <v-container>
      <v-sheet class="mx-auto" max-width="1000">
        <div
          class="mb-8"
          :class="[$vuetify.breakpoint.smAndUp ? 'text-h2' : 'text-h4']"
        >
          {{ title }}
        </div>
        <div class="text-subtitle-2">
          {{ description }}
        </div>
      </v-sheet>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      title:
        "We2Geda is a movement of millions of young patriotic Nigerians, coming together to make a lasting difference in nation-building.",
      description:
        "We represent a group of Nigerians between ages 18-50 years, home and abroad from diverse ethnic, religious, academic and professional backgrounds with the competence and experience required to drive the much-needed change of the Nigerian State. [We have a unified interest to initiate and commence a citizens-based engagement, which avails inclusion and merit in the processes by which we hope to be governed"
    };
  }
};
</script>

<style></style>
