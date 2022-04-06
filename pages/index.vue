<template>
<div>
  <Header />
  <Main />
  <PacotesIndex />
</div>
</template>

<script>
import Header from "~/components/Header.vue";
import Main from "~/components/Main.vue";
import PacotesIndex from '~/components/PacotesIndex.vue';
export default {
  components: { Header, Main, PacotesIndex },
  name: "IndexPage",
};
</script>
