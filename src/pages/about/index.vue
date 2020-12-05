<template>
  <div>
    <Hero backgroundImage="about.png" />
    <MoreAbout />
    <Vision />
    <Mission />
    <Cards />
    <Goal />
  </div>
</template>

<script>
import Hero from "~/components/Hero";
import MoreAbout from "~/components/Layouts/AboutLayout/MoreAbout";
import Vision from "~/components/Layouts/AboutLayout/Vision";
import Mission from "~/components/Layouts/AboutLayout/Mission";
import Cards from "~/components/Layouts/AboutLayout/Cards";
import Goal from "~/components/Layouts/AboutLayout/Goal";

export default {
  components: {
    Hero,
    MoreAbout,
    Vision,
    Mission,
    Cards,
    Goal
  }
};
</script>

<style></style>
