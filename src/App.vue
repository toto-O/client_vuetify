<template>
  <v-app>
    <v-main>
      <!-- <HelloWorld /> -->
      <v-container>
        <v-card>
          <v-app-bar></v-app-bar>
          <InputTextBox v-model="input_value" />
          {{ input_value }}
        </v-card>
      </v-container>
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
import { ref } from "vue";
// import HelloWorld from '@/components/HelloWorld.vue'
import InputTextBox from "@/components/InputTextBox.vue";

const input_value = ref<string>("hello");
</script>
