<template>
  <v-sheet>
    <div v-for="(item, i) in posts" :key="i">
      <v-sheet outlined class="mb-6">
        <v-row>
          <v-col cols="12" sm="6" md="4" class="py-0">
            <v-sheet
              class="image mb-2 fill-height"
              min-height="200"
              :style="`background-image: url(${item.image})`"
            >
            </v-sheet>
          </v-col>
          <v-col cols="12" sm="6" md="8">
            <v-sheet class="fill-height pa-4">
              <div class="text-h5 mb-4">
                {{ item.title }}
              </div>
              <div class="text-body-2 mb-4">
                {{ item.description }}
              </div>
              <v-btn
                depressed
                x-large
                class="transparent accent--text pl-0"
                :to="item.url"
                nuxt
              >
                <span class="text-decoration-underline">
                  See More
                </span>
                <v-icon right>
                  mdi-arrow-right
                </v-icon>
              </v-btn>
              <v-row>
                <v-col>
                  <div class="text-body-2 primary--text">
                    <v-icon class="mr-4" color="primary">
                      mdi-account
                    </v-icon>
                    {{ item.author }}
                  </div>
                </v-col>
                <v-spacer></v-spacer>
                <v-col>
                  <div class="text-body-2 primary--text">
                    <v-icon class="mr-4" color="primary">
                      mdi-calendar
                    </v-icon>
                    {{ item.date }}
                  </div>
                </v-col>
              </v-row>
            </v-sheet>
          </v-col>
        </v-row>
      </v-sheet>
    </div>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      posts: [
        {
          id: "1212",
          image: "/images/puzzle.jpg",
          title: "Post Title",
          description:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quas tempora aliquid possimus qui in reprehenderit nihil et ut, explicabo nisi fugit voluptatum aperiam minima, id, optio repudiandae vitae? Quaerat, quisquam.",
          link: "/",
          author: "Lorem",
          date: "1 Nov 2020"
        },
        {
          id: "1212",
          image: "/images/puzzle.jpg",
          title: "Post Title",
          description:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quas tempora aliquid possimus qui in reprehenderit nihil et ut, explicabo nisi fugit voluptatum aperiam minima, id, optio repudiandae vitae? Quaerat, quisquam.",
          link: "/",
          author: "Lorem",
          date: "1 Nov 2020"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.image {
  background-color: rgba($color: $light-grey, $alpha: 0.65);
  //   background-color: rgba($color: $dark-grey, $alpha: 0.8);
  background-position: center center;
  background-repeat: no-repeat;
  background-blend-mode: hue;
  background-size: cover;
}
</style>
