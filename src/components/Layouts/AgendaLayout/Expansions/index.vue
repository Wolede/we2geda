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
                {{ item.subtitle }}
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
          subtitle: `Review of the National Constitution to address its defects and tackle topics such as devolution of power and effectual fiscal tribalism.`
        },
        {
          title: "Electoral Reform",
          subtitle:
            "Reform our poorly-functioned electoral system to a digitised system with a strong legal framework that serves its purpose in transparency, accountability and unity. "
        },
        {
          title: "Youth and Women",
          subtitle:
            "Create an enabling environment where our women and youths receive optimum education, health care, and security. "
        },
        {
          title: "Economy",
          subtitle:
            "Change the narrative of unemployment with an all-inclusive strategy, economic diversification, strengthen private sector partnerships and institutional support. Reform the economy to better support ease of doing business and the financial market."
        },
        {
          title: "21st Century Infrastructure",
          subtitle:
            "Revolutionize our transportation, power and technology sector to a global standard that guarantees affordability and accessibility for all."
        },
        {
          title: "Digitizing Nigeria",
          subtitle: ""
        },
        {
          title: "Human Capital Development",
          subtitle:
            "Drive workforce to meet the global demand for human capital especially in the areas of technology, agriculture, and natural and mineral resources."
        },
        {
          title: "Education",
          subtitle:
            "Forward momentum of our nation is tied to our knowledge base, therefore, we must make efforts for education in Nigeria to be deliberate and strategic."
        },
        {
          title: "Agriculture and Food Security",
          subtitle:
            "Revamp our endowed agricultural sector to effortlessly accommodate our local food demand and gain revenue  from international trade."
        },
        {
          title: "Affordable Healthcare",
          subtitle:
            "A fully functional healthcare system is a top tier priority for good governance and should never be negotiable. The goal is to optimize and automate our healthcare system and pave the way for medical tourism."
        },
        {
          title: "Governance and Public Service Reform",
          subtitle:
            "A holistic reform of the public service accompanied with capacity development and digitization of the human resource and welfare process to achieve transparency and accountability."
        },
        {
          title: "Anti-Corruption and Justice",
          subtitle:
            "The continuous battle against corruption is profound, yet we remain incapaciteted by this menace. By launching a comprehensive anti-corruption strategy, supporting anti-corruption agencies and aligning the justice and legal components, we create a headway towards defeating corruption in our nation."
        },
        {
          title: "National Security",
          subtitle:
            "Clear cut -out strategies that curb all the factors threatening our national security with the aim of ensuring continuous peace and stability in our nation."
        },
        {
          title: "Social Security",
          subtitle:
            "Review and implemnet policies and programmes that not only solve the challanhes of poverty and vunlirebility over the life cycle of a Nigeria but also srenghten pro-poor and inclusive economic growth and socila development."
        }
      ]
    };
  }
};
</script>

<style></style>
