<template>
  <q-layout view="lHh Lpr lFf">
    <Header />
    <hr style="margin: 0"/>
    <router-view></router-view>
    <Footer />
  </q-layout>
</template>

<script>
import { ref } from "vue";
import Header from "@/components/Layout/Header";
import Footer from './components/Layout/Footer.vue';

export default {
  name: "LayoutDefault",

  components: {
    Header,
    Footer,
  },

  setup() {
    return {
      leftDrawerOpen: ref(false),
    };
  },
};
</script>

<style lang="scss">
.max-center {
  margin: auto;
  max-width: 1200px;
  width: 100%;
}
</style>
