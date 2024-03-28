<template>
  <q-card flat class="text-center q-mx-md">
    <q-icon size="lg" :name="data.icon" />
    <p class="text-h4 q-mt-md">{{ data.title }}</p>
    <p class="text-body1">
      {{ data.text }}
    </p>
  </q-card>
</template>

<script>
export default {
  props: {
    data: {
      type: Object
    }
  }
};
</script>
