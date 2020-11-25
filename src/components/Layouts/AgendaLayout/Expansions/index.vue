<template>
  <v-sheet class="pb-10">
    <v-container>
      <v-sheet class="mx-auto" max-width="1040">
        <v-expansion-panels focusable dark flat tile popout>
          <v-expansion-panel v-for="(item, i) in agendas" :key="i" class="mb-4">
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
      agendas: [
        {
          title: "Constitution Review",
          subtitle: ""
        },
        {
          title: "Electoral Reform",
          subtitle: ""
        },
        {
          title: "Youth and Women",
          subtitle: ""
        },
        {
          title: "Economy",
          subtitle: ""
        },
        {
          title: "21st Century Infrastructure",
          subtitle: ""
        },
        {
          title: "Digitizing Nigeria",
          subtitle: ""
        },
        {
          title: "Human Capital Development",
          subtitle: ""
        },
        {
          title: "Education",
          subtitle: ""
        },
        {
          title: "Agriculture and Food Security",
          subtitle: ""
        },
        {
          title: "Affordable Healthcare",
          subtitle: ""
        },
        {
          title: "Governance and Public Service Reform",
          subtitle: ""
        },
        {
          title: "Anti-Corruption and Justice",
          subtitle: ""
        },
        {
          title: "National Security",
          subtitle: ""
        },
        {
          title: "Social Security",
          subtitle: ""
        }
      ]
    };
  }
};
</script>

<style></style>
