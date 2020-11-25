<template>
  <div>
    <Hero backgroundImage="hero.jpg" />
    <Communities />
    <VolunteerForm />
  </div>
</template>

<script>
import Hero from "~/components/Hero";
import Communities from "~/components/Layouts/GetInvolvedLayout/Communities";
import VolunteerForm from "~/components/Layouts/GetInvolvedLayout/VolunteerForm";

export default {
  components: {
    Hero,
    Communities,
    VolunteerForm
  }
};
</script>

<style></style>
