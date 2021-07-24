<template>
  <div class="home">
    <div class="video-container">
      <video
        class="video"
        autoplay
        muted
        loop
        playsinline
        src="@/assets/videos/pk-digital-dental-lab.mp4"
      ></video>
      <img src="@/assets/images/logo.png" />
    </div>
    <ImageContainer
      leftSingle="pfm.png"
      leftTextSingle="PFM CROWN BRIDGE"
      leftDouble="01.jpg"
      leftTextDouble=""
      rightDouble="01.jpg"
      rightTextDouble=""
    />
    <div class="product-section">
      <div class="text-center max-center q-py-lg">
        <h3 class="q-my-sm">
          Premium Dentistry Services
        </h3>
        <h6 class="q-my-sm">
          A toothbrush, interdental brushes and toothpaste. That’s all you need.
          Or is it?
        </h6>
      </div>
      <div class="row justify-center max-center">
        <div class="column items-center col col-xs-12 col-sm-6">
          <div class="image-container">
            <img class="prod-image" src="@/assets/images/products/01.png" />
          </div>
          <div class="text-container">
            <h6 class="text-body1 q-my-sm">
              …THAT LOVE THE GUMLINE
            </h6>
            <h3 class="q-my-sm">
              TOOTHBRUSH
            </h3>
            <h6 class="q-my-sm">
              Brushing your teeth is also about cleaning your gumline. The
              sulcus – the groove between the teeth and gums – is a breeding
              ground for bacteria that cause inflammation and periodontitis. Our
              toothbrushes are so gentle, they clean perfectly – even in the
              gumline.
            </h6>
          </div>
        </div>
        <div class="column items-center col col-xs-12 col-sm-6">
          <div class="image-container">
            <img class="prod-image" src="@/assets/images/products/01.png" />
          </div>
          <div class="text-container">
            <h6 class="text-body1 q-my-sm">
              …THAT LOVE THE GUMLINE
            </h6>
            <h3 class="q-my-sm">
              TOOTHBRUSH
            </h3>
            <h6 class="q-my-sm">
              Brushing your teeth is also about cleaning your gumline. The
              sulcus – the groove between the teeth and gums – is a breeding
              ground for bacteria that cause inflammation and periodontitis. Our
              toothbrushes are so gentle, they clean perfectly – even in the
              gumline.
            </h6>
          </div>
        </div>
      </div>
      <div class="row justify-center max-center">
        <div class="column items-center col col-xs-12 col-sm-6">
          <div class="image-container">
            <img class="prod-image" src="@/assets/images/products/01.png" />
          </div>
          <div class="text-container">
            <h6 class="text-body1 q-my-sm">
              …THAT LOVE THE GUMLINE
            </h6>
            <h3 class="q-my-sm">
              TOOTHBRUSH
            </h3>
            <h6 class="q-my-sm">
              Brushing your teeth is also about cleaning your gumline. The
              sulcus – the groove between the teeth and gums – is a breeding
              ground for bacteria that cause inflammation and periodontitis. Our
              toothbrushes are so gentle, they clean perfectly – even in the
              gumline.
            </h6>
          </div>
        </div>
        <div class="column items-center col col-xs-12 col-sm-6">
          <div class="image-container">
            <img class="prod-image" src="@/assets/images/products/01.png" />
          </div>
          <div class="text-container">
            <h6 class="text-body1 q-my-sm">
              …THAT LOVE THE GUMLINE
            </h6>
            <h3 class="q-my-sm">
              TOOTHBRUSH
            </h3>
            <h6 class="q-my-sm">
              Brushing your teeth is also about cleaning your gumline. The
              sulcus – the groove between the teeth and gums – is a breeding
              ground for bacteria that cause inflammation and periodontitis. Our
              toothbrushes are so gentle, they clean perfectly – even in the
              gumline.
            </h6>
          </div>
        </div>
      </div>
    </div>
    <ImageContainer
      leftDouble="01.jpg"
      rightDouble="01.jpg"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import ImageContainer from "@/components/General/ImageContainer.vue";

export default defineComponent({
  components: { ImageContainer },
  name: "Home",
});
</script>

<style lang="scss">
.home {
  .video-container {
    max-height: 600px;
    overflow: hidden;
  }
  .video {
    width: 100%;
    height: 50%;
    object-fit: cover;
  }
  .product-section {
    background-color: #fbf4f8;
    .image-container {
      background-color: white;
      border-radius: 5%;
      max-width: 450px;
      max-height: 350px;
      margin: 50px 50px 0 50px;
      width: 100%;
      overflow: hidden;
    }
    .text-container {
      margin: 0px 50px;
      max-width: 450px;
      padding: 10px;
      overflow: hidden;
    }
    .prod-image {
      max-height: 350px;
      width: 100%;
      object-fit: contain;
    }
  }
}
</style>
