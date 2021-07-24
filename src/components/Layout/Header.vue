<template>
  <div class="sub-header">
    <div class="row q-py-xs q-mx-sm justify-between">
      <div class="row">
        <img class="flag" src="@/assets/images/Pakistan.png" />
        <h6 class="text-body2 q-ma-sm">
          Pakistan's premium dental restorations / Free delivery for all orders!
        </h6>
      </div>
      <h6 class="text-body2 q-ma-sm">ISLAMABAD | PESHAWAR | KABUL</h6>
    </div>
  </div>
  <div class="header">
    <div class="row justify-between max-center">
      <router-link to="/">
        <img
          class="logo"
          src="@/assets/images/logo.png"
          alt="chughtai-dental-lab"
        />
      </router-link>
      <nav class="q-my-auto">
        <ul class="row">
          <li v-for="(route, i) in routes" :key="i">
            <q-btn
              size="16px"
              class="q-mx-sm"
              :label="route.name"
              :to="route.path"
              unelevated
            />
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script lang="ts">
import { computed, defineComponent } from "vue";
import { useRouter } from "vue-router";
export default defineComponent({
  setup() {
    const router = useRouter();

    const routes = computed(() => {
      return router.options.routes;
    });

    return {
      routes,
    };
  },
});
</script>

<style lang="scss">
.sub-header {
  .flag {
    max-width: 45px;
    width: 100%;
  }
  background-color: #3d3d3d;
  color: white;
}
.header {
  background-color: #fbf4f8;
  .logo {
    max-width: 150px;
    width: 100%;
  }
  nav {
    li {
      list-style-type: none;
    }
  }
}
</style>
