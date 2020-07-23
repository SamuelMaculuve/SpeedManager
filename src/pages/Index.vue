<template>
  <q-page class="flex flex-center">
<!--    <img-->
<!--      alt="Quasar logo"-->
<!--      src="~assets/quasar-logo-full.svg"-->
<!--    >-->
    <detected-speed>
    <span slot="unknown">
      REEE! Unable to identify your network type.
    </span>
      <span slot="slow">
      <img src="cat.gif" alt="you got slow internet">
    </span>
      <span slot="fast">
      <video width="400" controls>
        <source src="mov_bbb.mp4" type="video/mp4">
        <source src="mov_bbb.ogg" type="video/ogg">
        Your browser does not support HTML5 video.
      </video>
    </span>
    </detected-speed>
  </q-page>
</template>

<script>
  import DetectedSpeed from 'vue-identify-network';
export default {
  name: 'PageIndex',
  components: {
    DetectedSpeed,
  },
}
</script>
