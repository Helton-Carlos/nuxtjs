<template>
<div>
  <Header />
  <Main />
  <PacotesIndex />
  <PasseiosIndex />
</div>
</template>

<script>
import Header from "~/components/Header.vue";
import Main from "~/components/Main.vue";
import PacotesIndex from '~/components/PacotesIndex.vue';
import PasseiosIndex from '~/components/PasseiosIndex.vue';
export default {
  components: { Header, Main, PacotesIndex, PasseiosIndex },
  name: "IndexPage",
   asyncData() {
    console.log("hey");
  },
};
</script>
