<template>
  <v-sheet>
    <div class="text-h5" v-if="showTitle">
      {{ title }}
    </div>
    <div class="pr-10">
      <div v-for="(item, i) in socialLinks" :key="i">
        <v-btn
          depressed
          tile
          dark
          block
          x-large
          :color="item.color"
          class="justify-start my-4"
          :href="item.url"
          target="_blank"
        >
          <v-icon left> {{ item.icon }} </v-icon>
          <span class="text-uppercase">
            {{ item.name }}
          </span>
        </v-btn>
      </div>
    </div>
  </v-sheet>
</template>

<script>
export default {
  props: {
    showTitle: {
      type: Boolean,
      default: true
    }
  },
  data() {
    return {
      title: "Get in Touch",
      socialLinks: [
        {
          name: "facebook",
          icon: "mdi-facebook",
          url: "https://www.facebook.com/OfficialWe2Geda",
          color: "blue"
        },
        {
          name: "twitter",
          icon: "mdi-twitter",
          url: "https://twitter.com/officialwe2geda",
          color: "blue lighten-3"
        },
        {
          name: "instagram",
          icon: "mdi-instagram",
          url: "https://www.instagram.com/officialwe2geda/",
          color: "blue lighten-2"
        },
        {
          name: "whatsapp",
          icon: "mdi-whatsapp",
          url: "https://wa.me/2347064326402",
          color: "green"
        }
      ]
    };
  }
};
</script>

<style></style>
