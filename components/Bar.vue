<script setup lang="ts">
import { ref } from 'vue';
import Foo from './Foo.vue';
const foos = ref(null);
console.log('foo!');
const bar = 0;
</script>
<template>
  <Foo v-for="_ in 5" ref="foos" />
</template>
<style>
div {
  margin: v-bind(bar);
}
</style>
