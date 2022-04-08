<template>
  <div>
    <Header />
    <Main />
    <PacotesIndex />
    <PasseiosIndex />
    <Newslater />
    <PromocaoIndex />
    <Form />
    <RodaPe />
  </div>
</template>

<script>
import Header from "~/components/Header.vue";
import Main from "~/components/Main.vue";
import Newslater from "~/components/Newslater.vue";
import PacotesIndex from "~/components/PacotesIndex.vue";
import PasseiosIndex from "~/components/PasseiosIndex.vue";
import PromocaoIndex from "~/components/PromocaoIndex.vue";
import Form from "~/components/Form.vue";
import RodaPe from "~/components/RodaPe.vue";
export default {
  components: {
    Header,
    Main,
    PacotesIndex,
    PasseiosIndex,
    Newslater,
    PromocaoIndex,
    Form,
    RodaPe,
  },
  name: "IndexPage",
  asyncData() {
    console.log("hey");
  },
};
</script>
