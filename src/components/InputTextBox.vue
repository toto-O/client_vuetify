<template>
  <v-text-field label="label" v-model="update" />
</template>

<script setup lang="ts">
import { computed } from "vue";
const props = defineProps(["value"]);
const emit = defineEmits(["input"]);

const update = computed({
  get() {
    return props.value;
  },
  set() {
    emit("input", update);
  },
});
</script>
