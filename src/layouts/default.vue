<template>
  <v-app>
    <v-main>
      <Header />
      <nuxt />
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Header from "~/components/Header";
import Footer from "~/components/Footer";

export default {
  components: {
    Header,
    Footer
  },
  data() {
    return {};
  }
};
</script>
