<template>
  <div class="row q-mx-auto justify-center align-center">
    <div class="col-12 col-lg-6 self-center">
      <q-card flat class="q-pa-xl">
        <q-card-section class="text-h4">
          {{ title }}
        </q-card-section>
        <q-card-section>
          {{ text }}
        </q-card-section>
      </q-card>
    </div>
    <div class="col-12 col-lg-6">
      <q-img :src="img" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: "Why Us?"
    },
    text: {
      type: String,
      default:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam cupiditate ex earum soluta accusantium id corrupti sit deserunt dolorem ut, eius, numquam illo perferendis, reiciendis tempore quis at libero laudantium?"
    },
    img: {
      type: String
    }
  }
};
</script>

<style></style>
