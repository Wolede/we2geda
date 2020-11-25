<template>
  <v-sheet color="secondary" class="py-10">
    <v-container>
      <v-row>
        <v-col cols="12" sm="4" md="4" v-for="(value, i) in values" :key="i">
          <v-sheet :class="value.color" dark class="pa-6 fill-height">
            <div class="text-h5 mb-6">
              {{ value.title }}
            </div>
            <div class="text-body-2">
              {{ value.desc }}
            </div>
          </v-sheet>
        </v-col>
      </v-row>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      values: [
        {
          color: "accent",
          title: "Love",
          desc:
            "Our principal driving force is love which encompasses love for self, for our community, and our great nation and for all it could be. With love as our foundation, many of the despicable acts being perpetrated by public officers will be obsolete. We will act in love for the betterment of each other and our nation as a whole."
        },
        {
          color: "dark",
          title: "Respect",
          desc:
            "Our principal driving force is love which encompasses love for self, for our community, and our great nation and for all it could be. With love as our foundation, many of the despicable acts being perpetrated by public officers will be obsolete. We will act in love for the betterment of each other and our nation as a whole."
        },
        {
          color: "accent",
          title: "Justice",
          desc:
            "We shall operate on the principle of justice and fairness - just treatment without favouritism or discrimation irrespective of tribe, faith and political affiliation and uphold the laws of the land."
        },
        {
          color: "primary",
          title: "Empathy",
          desc:
            "We want to foster a government-citizen relationship where leaders are in sync with the needs, desires, aspirations and groanings of the people; a kind of relationship where leaders can rightly respond because they can truly understand."
        },
        {
          color: "accent",
          title: "Integrity",
          desc:
            "We want to build a Nation premised on the culture of integrity. A place with people who have a guiding moral compass and know the difference between right and wrong, people who will carry out their duties with that same spirit, and refuse to condone contrary behaviour."
        },
        {
          color: "dark",
          title: "Accountability / Diligence",
          desc:
            "We place great importance on being diligent and aim to build a system with effective checks and balances, to ensure accountability. We are guided by the call to serve the benefit of all people of Nigeria, and we will do so with agility, promptness and diligence."
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.dark {
  background-color: $dark-grey;
}
</style>
