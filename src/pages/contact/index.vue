<template>
  <div>
    <Hero backgroundImage="man.jpg" />
    <v-container>
      <v-row>
        <v-col cols="12" sm="12" md="4">
          <MediaButtons :showTitle="false" />
        </v-col>
        <v-col cols="12" sm="12" md="8">
          <ContactDetails />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import Hero from "~/components/Hero";
import MediaButtons from "~/components/Layouts/NewsLayout/MediaButtons";
import ContactDetails from "~/components/Layouts/ContactLayout/ContactDetails";

export default {
  components: {
    Hero,
    MediaButtons,
    ContactDetails
  }
};
</script>

<style></style>
