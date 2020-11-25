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
        <div
          class="text-subtitle-2 mb-6"
          v-for="(description, i) in descriptions"
          :key="i"
        >
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
      title: "Agenda",
      descriptions: [
        "Our New-Nigeria agenda is built on hope, love, trust and harmony. We hope for a country where every Nigerian—irrespective of ethnicity,​ religion, class or political affiliation ​can live a secure, safe, and healthy life, with access to fair and equitable opportunities to provide for their families, and the ability to participate in achieving a people-centric government.",
        "Using this platform, we are crowdsourcing policy ideas, input and contributions from you all."
      ]
    };
  }
};
</script>

<style></style>
