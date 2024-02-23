<script setup>
import { RouterView, useRoute } from 'vue-router'
import Default from './layouts/default.vue'
import Blank from './layouts/blank.vue'
const route = useRoute()

</script>

<template>
  <Default v-if="route.meta.layout !== 'blank'" />
  <Blank v-if="route.meta.layout === 'blank'" />
  <RouterView />
</template>

<style scoped></style>
