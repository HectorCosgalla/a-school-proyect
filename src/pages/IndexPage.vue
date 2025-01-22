<template>
  <q-page class="flex flex-center">
    <q-tabs v-model="tab" no-caps class="folder-selector text-white shadow-2">
      <q-tab class="folder" name="mails" label="Mails" />
      <q-tab name="alarms" label="Alarms" />
      <q-tab name="movies" label="Movies" />
    </q-tabs>
  </q-page>
</template>

<script setup>
import { ref } from 'vue'

const tab = ref('mails')
</script>

<style>
.folder-selector {
  background-color: aqua;
}

.folder {
  margin: 5% 10%;
  background-color: red;
}
</style>
