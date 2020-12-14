<template>
  <v-sheet class="py-10" dark>
    <v-container>
      <v-row justify="space-between">
        <v-col cols="12" sm="12" md="6">
          <Logo />
        </v-col>
        <v-col cols="12" sm="12" md="6" class="d-flex flex-column align-end">
          <div>
            <div class="text-caption font-weight-bold info--text mb-4">
              Contact
            </div>
            <div class="text-caption info--text mb-2">
              Phone:
              <a
                href="tel:+234 (0) 12299504"
                class="text-caption info--text font-weight-bold link"
              >
                +234 (0) 12299504</a
              >
            </div>
            <div class="text-caption info--text mb-2">
              Email: <span class="font-weight-bold"></span>
              <a
                href="mailto:connect@we2geda.ng"
                class="text-caption info--text font-weight-bold link"
                >connect@we2geda.ng</a
              >
            </div>
            <div class="text-caption info--text my-2 d-flex align-center">
              <span>
                Social:
              </span>
              <span class="d-flex justify-space-between align-center">
                <v-btn
                  v-for="(item, i) in socialLinks"
                  :key="i"
                  color="transparent"
                  fab
                  depressed
                  small
                  dark
                  :href="item.url"
                  target="_blank"
                  class="mx-1 icon-wrap"
                >
                  <!-- <v-icon> {{ item.icon }} </v-icon> -->
                  <img :src="item.icon" :alt="item.name" class="icon-image">
                </v-btn>
              </span>
            </div>
          </div>
        </v-col>
      </v-row>
      <v-divider class="my-6"></v-divider>
      <v-row>
        <v-col cols="12" sm="4" md="4">
          <div class="text-caption info--text mb-2 text-center border-right">
            Paid for by We Together Nigeria
          </div>
        </v-col>
        <v-col cols="12" sm="4" md="4">
          <div class="text-center border-right">
            <span class="info--text"
              >&copy; {{ new Date().getFullYear() }}</span
            >
            <span class="text-caption info--text">
              We2gedaNG. All Rights Reserved
            </span>
          </div>
        </v-col>
        <v-col cols="12" sm="4" md="4">
          <div class="text-caption info--text mb-2 text-center border-right">
            In Loving Memory of our Founding Fathers
          </div>
        </v-col>
      </v-row>
      <!-- <v-row justify="center">
        <v-col cols="12" sm="4" md="2">
          <div class="text-caption info--text mb-2 text-right">
            Terms
          </div>
        </v-col>
        <v-col cols="12" sm="4" md="2">
          <div class="text-caption info--text mb-2">
            Privacy
          </div>
        </v-col>
      </v-row> -->
    </v-container>
  </v-sheet>
</template>

<script>
import Logo from "~/components/Logo";

export default {
  components: {
    Logo
  },
  data() {
    return {
      socialLinks: [
        {
          name: "facebook",
          icon: "/images/facebook.svg",
          url: "https://www.facebook.com/OfficialWe2Geda"
        },
        {
          name: "twitter",
          icon: "/images/twitter.svg",
          url: "https://twitter.com/officialwe2geda"
        },
        {
          name: "instagram",
          icon: "/images/instagram.svg",
          url: "https://www.instagram.com/officialwe2geda/"
        },
        {
          name: "whatsapp",
          icon: "/images/whatsapp.svg",
          url: "https://wa.me/2347064326402"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.footer {
  background-color: $dark-grey;
}
.icon-wrap {
  display: flex;
  justify-content: center;
  align-items: center;
}
.icon-image{
  height: 30px;
  width: 30px;
}
.border-right{
  border-right: 1px solid rgba(255, 255, 255, 0.12);
}
</style>
