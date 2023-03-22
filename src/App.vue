<script setup>
import { ref } from "vue";
// import LzTable from "jiangzhen-components/src/components/lz-table/index.vue";
import { LzTable } from "jiangzhen-components";

const count = ref(0);

function increment() {
  count.value++;
}
</script>

<template>
  <div>
    <h3>{{ count }}</h3>
    <button @click="increment">click</button>
    <LzTable :num="count" />
  </div>
</template>
