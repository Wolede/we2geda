<template>
  <div>
    <Hero backgroundImage="agenda.jpg" />
    <MoreAgenda />
    <Expansions />
    <ContributeForm />
  </div>
</template>

<script>
import Hero from "~/components/Hero";
import MoreAgenda from "~/components/Layouts/AgendaLayout/MoreAgenda";
import Expansions from "~/components/Layouts/AgendaLayout/Expansions";
import ContributeForm from "~/components/Layouts/AgendaLayout/ContributeForm";

export default {
  components: {
    Hero,
    MoreAgenda,
    Expansions,
    ContributeForm
  }
};
</script>

<style></style>
