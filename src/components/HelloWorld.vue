<script setup lang="ts">
import { SelfieSegmentation, VERSION } from "@mediapipe/selfie_segmentation";

defineProps<{ msg: string }>();

console.log("Lib", SelfieSegmentation);
console.log("VERSION", VERSION);
</script>

<template>
  <h1>{{ msg }}</h1>
  <h2>This is minimal reproduction of existing bug</h2>

  <br />
  <div>import SelfieSegmentation - {{ typeof SelfieSegmentation }}</div>
  <div>import Version of selfie segmentation - {{ VERSION }}</div>
</template>

<style scoped></style>
