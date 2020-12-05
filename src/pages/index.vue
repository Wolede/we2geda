<template>
  <div>
    <Hero page="home" backgroundImage="home-header.png" />
    <HomeAbout />
    <JoinForm />
    <JoinHighlight />
    <JoinUs />
  </div>
</template>

<script>
import Hero from "~/components/Hero";
import HomeAbout from "~/components/Layouts/HomeLayout/About";
import JoinForm from "~/components/Layouts/HomeLayout/JoinForm";
import JoinHighlight from "~/components/Layouts/HomeLayout/JoinHighlight";
import JoinUs from "~/components/Layouts/HomeLayout/JoinUs";

export default {
  components: {
    Hero,
    HomeAbout,
    JoinForm,
    JoinHighlight,
    JoinUs
  }
};
</script>
