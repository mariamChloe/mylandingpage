<template>
  <div class="row q-ma-md q-pa-xl">
    <div class="col-12 col-lg-4" :key="index" v-for="(d, index) in data">
      <Feature :data="d" />
    </div>
  </div>
</template>

<script>
import Feature from "../components/Feature";

export default {
  props: {
    data: {
      type: Array
    }
  },
  components: {
    Feature
  }
};
</script>

<style></style>
