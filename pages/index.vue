<template>
<div>
  <Header />
  <Main />
  <Pacotes />
</div>
</template>

<script>
import Header from "~/components/Header.vue";
import Main from "~/components/Main.vue";
import Pacotes from '~/components/Pacotes.vue';
export default {
  components: { Header, Main, Pacotes },
  name: "IndexPage",
};
</script>
