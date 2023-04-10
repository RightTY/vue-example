<script lang="ts" setup>
import { ref } from "vue";

const object = { foo: ref(1), too: ref(2) };
const { foo } = object;
const { too } = object;
function increment() {
  foo.value++;
}
function increment1() {
  too.value++;
}
</script>

<template>
  <button @click="increment">{{ object.foo.value + 1 }}</button>
  <button @click="increment">{{ foo + 1 }}</button>
  <button @click="increment1">{{ too + 1 }}</button>
</template>
