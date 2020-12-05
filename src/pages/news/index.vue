<template>
  <div>
    <Hero backgroundImage="pic-2.jpg" />
    <Activity />
    <v-container>
      <v-row>
        <v-col cols="12" sm="12" md="4">
          <MediaButtons />
        </v-col>
        <v-col cols="12" sm="12" md="8">
          <Posts />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import Hero from "~/components/Hero";
import Activity from "~/components/Layouts/NewsLayout/Activity";
import MediaButtons from "~/components/Layouts/NewsLayout/MediaButtons";
import Posts from "~/components/Layouts/NewsLayout/Posts";

export default {
  components: {
    Hero,
    Activity,
    MediaButtons,
    Posts
  }
};
</script>

<style></style>
