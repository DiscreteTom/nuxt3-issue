<template>
  <div>
    <div class="d-flex flex-wrap">
      <v-card
        v-for="(value, name) in result"
        :key="name"
        class="mx-2 my-2 flex-grow-1"
      >
        <v-card-title class="d-flex align-center"> </v-card-title>
        <v-card-text>
          {{ value }}
        </v-card-text>
      </v-card>
    </div>
  </div>
</template>

<script setup lang="ts">
const result = reactive({
  key: "",
});

onMounted(() => {
  result.key = "value";
});
</script>
