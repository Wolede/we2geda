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
            <div class="text-caption info--text my-2">
              <span>
                Social:
              </span>
              <span>
                <v-btn
                  v-for="(item, i) in socialLinks"
                  :key="i"
                  color="primary"
                  fab
                  depressed
                  x-small
                  dark
                  class="mx-1"
                  :href="item.url"
                  target="_blank"
                >
                  <v-icon> {{ item.icon }} </v-icon>
                </v-btn>
              </span>
            </div>
          </div>
        </v-col>
      </v-row>
      <v-divider class="my-6"></v-divider>
      <v-row>
        <v-col cols="12" sm="4" md="4">
          <div class="text-caption info--text mb-2 text-center">
            Paid for by We Together Nigeria
          </div>
        </v-col>
        <v-col cols="12" sm="4" md="4">
          <div class="text-center">
            <span class="info--text"
              >&copy; {{ new Date().getFullYear() }}</span
            >
            <span class="text-caption info--text">
              We2gedaNG. All Rights Reserved
            </span>
          </div>
        </v-col>
        <v-col cols="12" sm="4" md="4">
          <div class="text-caption info--text mb-2 text-center">
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
          icon: "mdi-facebook",
          url: ""
        },
        {
          name: "twitter",
          icon: "mdi-twitter",
          url: ""
        },
        {
          name: "instagram",
          icon: "mdi-instagram",
          url: ""
        },
        {
          name: "whatsapp",
          icon: "mdi-whatsapp",
          url: "https://wa.me/1XXXXXXXXXX"
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
</style>
