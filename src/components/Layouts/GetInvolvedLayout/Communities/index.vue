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
      </v-sheet>
      <v-sheet class="mx-auto" max-width="1040">
        <v-expansion-panels focusable dark flat tile popout>
          <v-expansion-panel v-for="(item, i) in units" :key="i" class="mb-4">
            <v-expansion-panel-header color="secondary">
              <div class="text-h5">{{ item.title }}</div>
            </v-expansion-panel-header>
            <v-expansion-panel-content color="secondary">
              <div class="text-subtitle-2">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat.
              </div>
              <div class="d-flex justify-end">
                <v-btn
                  depressed
                  x-large
                  class="transparent accent--text pl-0 mt-6"
                  href="https://forms.google.com"
                  target="_blank"
                >
                  <span class="text-decoration-underline">
                    Find out more
                  </span>
                  <v-icon right>
                    mdi-arrow-right
                  </v-icon>
                </v-btn>
              </div>
            </v-expansion-panel-content>
          </v-expansion-panel>
        </v-expansion-panels>
      </v-sheet>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      title: "Steering Unit",
      units: [
        {
          title: "National Project Management Unit",
          desc: "",
          link: ""
        },
        {
          title: "Legal Steering Unit",
          desc: "",
          link: ""
        },
        {
          title: "Research & Strategy Steering Unit",
          desc: "",
          link: ""
        },
        {
          title: "Communications & Media Steering Unit",
          desc: "",
          link: ""
        },
        {
          title: "Finance Steering Unit",
          desc: "",
          link: ""
        },
        {
          title: "Political Steering Unit",
          desc: "",
          link: ""
        },
        {
          title: "NGO & CSO Steering Unit",
          desc: "",
          link: ""
        },
        {
          title: "Diaspora & Development Partners",
          desc: "",
          link: ""
        },
        {
          title: "Contact and Mobilization Steering Unit",
          desc: "",
          link: ""
        },
        {
          title: "Monitoring & Evaluation Steering Unit",
          desc: "",
          link: ""
        }
      ]
    };
  }
};
</script>

<style></style>
