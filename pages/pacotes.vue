<template>
  <div>
    <Header />
    <PacotesIndex />
  </div>
</template>

<script>
import Header from "~/components/Header.vue";
import PacotesIndex from '~/components/PacotesIndex.vue';
export default {
  name: "pacotes",
  components: { Header,PacotesIndex},
};
</script>

<style></style>
