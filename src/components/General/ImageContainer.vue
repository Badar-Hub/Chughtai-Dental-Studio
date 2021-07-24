<template>
  <div
    v-if="leftSingle"
    class="large-image-box max-center image-box q-my-md"
  >
    <div class="row max-center q-py-lg">
      <div class="col col-xs-12 col-sm-6 q-pa-md">
        <div class="image-container">
          <h6 class="q-px-md q-my-sm">{{ leftTextSingle }}</h6>
          <span>
            <q-btn size="md" to="/" label="Learn More >" unelevated />
          </span>
        </div>
      </div>
      <div class="column justify-center items-center col col-xs-12 col-sm-6">
        <div class="image-container">
          <img
            class="image"
            :src="require(`@/assets/images/categories/${leftSingle}`)"
          />
        </div>
      </div>
    </div>
  </div>
  <div
    v-if="leftDouble && rightDouble"
    class="image-box q-py-md"
  >
    <div class="row justify-between max-center">
      <div class="column items-start col col-xs-12 col-sm-6">
        <div class="image-container text-left">
          <img
            class="image"
            :src="require(`@/assets/images/feature-items/${leftDouble}`)"
          />
        </div>
      </div>
      <div class="column items-end col col-xs-12 col-sm-6">
        <div class="image-container text-right">
          <img
            class="image"
            :src="require(`@/assets/images/feature-items/${rightDouble}`)"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    leftSingle: {
      type: String,
    },
    leftTextSingle: {
      type: String,
      default: () => "",
    },
    leftDouble: {
      type: String,
    },
    leftTextDouble: {
      type: String,
      default: () => "",
    },
    rightDouble: {
      type: String,
    },
    rightTextDouble: {
      type: String,
      default: () => "",
    },
  },
});
</script>

<style lang="scss">
.image-box {
  .image-container {
    max-width: 570px;
    width: 100%;
    overflow: hidden;
    .image {
      margin: auto;
      max-width: 570px;
      width: 100%;
      transition: background 0.25s ease;
      box-shadow: 0 3px 6px 0 rgb(0 0 0 / 10%);
    }
  }
}
.large-image-box {
  background-color: #d4d4d475 !important;
  transition: background 0.25s ease;
  box-shadow: 0 3px 6px 0 rgb(0 0 0 / 10%);
}
</style>
