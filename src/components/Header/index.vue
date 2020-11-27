<template>
  <div>
    <v-navigation-drawer v-model="drawer" right fixed app>
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          nuxt
          exact
        >
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <div class="header-wrap bg-white">
      <v-app-bar
        absolute
        flat
        color="transparent"
        dark
        hide-on-scroll
        scroll-target="#below-hero"
      >
        <v-container class="pa-0">
          <v-toolbar flat color="transparent" :dark="true" class="elevation-0">
            <!-- <v-app-bar-nav-icon> -->
            <Logo />
            <!-- </v-app-bar-nav-icon> -->

            <v-spacer></v-spacer>
            <v-toolbar-items class="hidden-xs-only">
              <v-btn
                v-for="(item, i) in items"
                :key="i"
                :to="item.to"
                depressed
                color="transparent"
                large
                >{{ item.title }}</v-btn
              >
            </v-toolbar-items>

            <v-spacer></v-spacer>
            <v-btn to="/donate" rounded depressed color="accent">Donate</v-btn>
            <v-app-bar-nav-icon
              class="hidden-sm-and-up"
              @click.stop="drawer = !drawer"
            />
          </v-toolbar>
        </v-container>
      </v-app-bar>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo";

export default {
  components: {
    Logo
  },
  data() {
    return {
      drawer: false,
      items: [
        {
          title: "About",
          to: "/about"
        },
        {
          title: "Agenda",
          to: "/agenda"
        },
        {
          title: "Get Involved",
          to: "/get-involved"
        },
        {
          title: "News",
          to: "/news"
        },
        {
          title: "Contact",
          to: "/contact"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.v-toolbar {
  height: auto !important;
  ::v-deep .v-toolbar__content {
    height: auto !important;
  }
  ::v-deep .v-toolbar__items {
    height: 64px;
  }
}
// .search {
//   min-width: 16rem;

//   @media screen and (max-width: 1280px) {
//     min-width: 10rem;
//   }
// }
</style>
